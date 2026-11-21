# Debugging from Test Explorer

This lesson adds a discount method and two tests for it. One of the tests fails, because the method has a bug.

Add a file to the Pricing project named Discounts.cs, and paste in this code:

```csharp
namespace Pricing;

public static class Discounts
{
    // Takes a percentage off a price. For example, 10 takes 10 percent off.
    public static decimal ApplyPercent(decimal price, decimal percent)
    {
        decimal discount = price * percent;
        return price - discount;
    }
}
```

Add a file to Pricing.Tests named DiscountsTests.cs, and paste in this code:

```csharp
using NUnit.Framework;
using Pricing;

namespace Pricing.Tests;

[TestFixture]
public class DiscountsTests
{
    [Test]
    public void ApplyPercent_TenPercentOffTwenty_IsEighteen()
    {
        decimal result = Discounts.ApplyPercent(20m, 10m);
        Assert.That(result, Is.EqualTo(18m));
    }

    [Test]
    public void ApplyPercent_ZeroPercent_LeavesPriceUnchanged()
    {
        decimal result = Discounts.ApplyPercent(20m, 0m);
        Assert.That(result, Is.EqualTo(20m));
    }
}
```

Build with {{Ctrl+Shift+B}}, and run all the tests with {{Ctrl+R}}, then {{A}}. The zero-percent test passes. The 10 percent test fails, and its message says the method returned -180 where 18 was expected.

Now debug the failing test. Open Discounts.cs, and press {{F9}} on the line that declares discount. In Test Explorer, right-click ApplyPercent_TenPercentOffTwenty_IsEighteen, and choose Debug Test(s), as Figure 13.1 shows.

![Figure 13.1 - Debug Test(s) on the right-click menu](images/ch13-debug-context-menu.png "width=60%")

*Figure 13.1 - Debug Test(s) on the right-click menu*

The debugger stops at your breakpoint, with the Locals window open. Figure 13.2 shows the values. Read price and percent. Then press {{F10}} once, and watch discount change.

![Figure 13.2 - The test stopped at a breakpoint, with the Locals window showing the values](images/ch13-test-stopped-locals.png "width=75%")

*Figure 13.2 - The test stopped at a breakpoint, with the Locals window showing the values*

## Try it

1. Add the two files, build, and run all the tests.
2. Set the breakpoint on the line that declares discount in Discounts.cs.
3. Right-click the failing test, and choose Debug Test(s). Read price and percent in the Locals window.
4. Press {{F10}}, and check the value of discount. Press {{Shift+F5}} to stop the debugger.
