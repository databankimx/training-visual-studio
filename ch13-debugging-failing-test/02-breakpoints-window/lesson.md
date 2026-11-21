# The Breakpoints window

A breakpoint that stops every time can be slow to use. When a method runs many times, you want the debugger to stop only in the case you are chasing. A condition does that. It is an expression that must be true before the breakpoint pauses the program.

Open PriceCalculator.cs in the Pricing project, and find the line inside the loop in Total, the line that reads `total += price;`. Press {{F9}} to set a breakpoint there. Right-click the red dot in the gutter, and choose Conditions. Type `price > 5m` in the box, and make sure the condition is set to be true.

Run PriceReport with {{F5}}. The program prints its prices as it goes, and the debugger pauses only for the prices above 5, which are 12.50, 8.00, and 20.00. The price 3.75 passes without a pause. Figure 13.3 shows the Breakpoints window, with the condition in its column.

![Figure 13.3 - The Breakpoints window with a condition on a breakpoint](images/ch13-breakpoints-window.png "width=75%")

*Figure 13.3 - The Breakpoints window with a condition on a breakpoint*

Open the Breakpoints window from the Debug menu, under Windows, or press {{Ctrl+Alt+B}}. It lists every breakpoint in the solution, with its file, line, and condition. Clear a box to turn a breakpoint off without deleting it.

## Try it

1. Set the breakpoint in Total, and add the condition price greater than 5.
2. Run PriceReport with {{F5}}. Note which prices the debugger stops for.
3. Open the Breakpoints window with {{Ctrl+Alt+B}}, and find the breakpoint and its condition.
4. Press {{Shift+F5}} to stop the program. Delete the breakpoint with {{F9}}.
