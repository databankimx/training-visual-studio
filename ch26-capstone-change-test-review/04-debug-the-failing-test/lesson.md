# Debug the failing test

Now find out why the code returns 9. Open `PriceCalculator.cs` in the Pricing project, and find `MinPrice`. Press {{F9}} on the line that returns the result, so the breakpoint stops before the method returns.

In Test Explorer, right-click `MinPrice_ReturnsTheSmallest`, and choose Debug Test(s). Visual Studio stops at the breakpoint. Open the Locals window, and read `prices`. Then step over the return line with {{F10}}, and watch what the method returns.

The method returns the largest value in the list, not the smallest. Read the code line by line: it calls `Max` where the method name says `Min`. That is a copy-paste mistake, and it is the kind of bug a test exists to catch.

Stop the debugger with {{Shift+F5}} when you finish.

## Try it

1. Set a breakpoint on the return line in `MinPrice` with {{F9}}.
2. Right-click `MinPrice_ReturnsTheSmallest` in Test Explorer, and choose Debug Test(s).
3. Read `prices` in the Locals window, then stop the debugger with {{Shift+F5}}.
