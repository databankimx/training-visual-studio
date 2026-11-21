# Homework: step through a wrong value

This exercise gives you a method with a bug in its loop. The method should add up the first three prices, but it returns the wrong sum. Step through the method, watch the values, and find the line that goes wrong.

## Set up the file

Create a new file in the Pricing project, named BuggySum.cs. Paste in this code, and save the file.

```csharp
namespace Pricing;

public static class BuggySum
{
    public static decimal SumFirst(IReadOnlyList<decimal> prices, int count)
    {
        decimal sum = 0m;
        for (int i = 1; i < count; i++)
        {
            sum += prices[i];
        }
        return sum;
    }
}
```

To call the method, add this line to the end of PriceReport/Program.cs, and remember to delete it when you finish:

`Console.WriteLine($"First three: {BuggySum.SumFirst(prices, 3)}");`

The first three prices are 12.50, 8.00, and 3.75, so the answer should be 24.25.

## Work through these steps in order

1. **Predict the answer.** Before you run the program, write down what you expect the output to be.
2. **Set a breakpoint.** Put a breakpoint on the line that declares sum, in BuggySum.cs.
3. **Start with F5.** Run PriceReport, and let the debugger stop at the breakpoint.
4. **Step through the loop.** Press {{F10}} and watch sum and i in the Locals window. Note the first value of i, and the first price it adds.
5. **Find the wrong value.** Compare the values with the list of prices. Write down the line where the value first differs from what you expect.

## Check your work

Fix the bug, build with {{Ctrl+Shift+B}}, and run with {{Ctrl+F5}}. The line should read 24.25.

When you are done, delete BuggySum.cs, and delete the line you added to Program.cs.

~~~spoiler
The loop starts at index 1, so the first price, 12.50, is never added. It also stops at index 2, which is the last of the three prices, so the sum includes 8.00 and 3.75 and no more.

The fix is to start the loop at 0:

```csharp
for (int i = 0; i < count; i++)
```

With that change, the sum is 12.50 + 8.00 + 3.75, which is 24.25.

In the debugger, the first value of i is 1, and the first price added is 8.00, not 12.50. That is the line where the value first differs from what you expect.
~~~
