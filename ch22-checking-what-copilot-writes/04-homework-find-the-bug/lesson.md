# Homework: find the bug Copilot explains wrongly

This exercise has a method with a bug in it. Copilot's explanation of the method is wrong. Your job is to find the bug yourself, prove it with a test, and fix it, without trusting the explanation.

## Step 1: create the file

In the Pricing project, create a file named Stats.cs, paste in this code, and save it:

```csharp
namespace Pricing;

public static class Stats
{
    public static decimal Mean(IReadOnlyList<decimal> values)
    {
        decimal sum = 0m;
        for (int i = 1; i < values.Count; i++)
        {
            sum += values[i];
        }
        return sum / values.Count;
    }
}
```

## Step 2: ask Copilot to explain it

Select the whole Mean method. In the Chat window, ask, What does this method return? Read the answer. It will probably say the method adds every value and divides by the count. Write that claim down, because you are going to test it.

## Step 3: write a test

In Pricing.Tests, create StatsTests.cs, with a test that works out the answer by hand:

```csharp
using NUnit.Framework;
using Pricing;

namespace Pricing.Tests;

[TestFixture]
public class StatsTests
{
    [Test]
    public void Mean_OfTwoFourSix_IsFour()
    {
        decimal result = Stats.Mean(new[] { 2m, 4m, 6m });
        Assert.That(result, Is.EqualTo(4m));
    }
}
```

Build with {{Ctrl+Shift+B}}, and run the test from Test Explorer. Read the failure message. Does the method return what Copilot's explanation said?

## Step 4: find the bug

Look at the loop. Work out which values it adds, and which it skips. Write the bug in one sentence, in your own words.

## Step 5: fix it, and decide the empty list

Change the loop so it adds every value. Run all the tests. Then decide what Mean should do for an empty list. Right now, dividing by zero throws an exception. Either document that in a comment, or add a check that returns zero, and write a test for it.

Stage and commit the change, with the message Fix Mean to include every value.

~~~spoiler
The bug is the starting index. The loop begins at index 1, so it skips the first value, 2. For the list 2, 4, and 6, it adds 4 and 6, which is 10, and divides by three. The method returns 3.33 instead of 4.

Copilot's explanation said the method adds every value, which is wrong. That mismatch is why this homework exists.

The fix is to start the loop at index 0:

```csharp
for (int i = 0; i < values.Count; i++)
```

For an empty list, the sum is zero, and the division by zero throws an exception. A simple choice is an explicit check at the top of the method, which returns zero when the list is empty, plus a test that checks it.
~~~
