# Breakpoints

A breakpoint tells the debugger to pause the program when it reaches a line. Put the cursor on the line, and press {{F9}}. A red dot appears in the gutter, the narrow strip to the left of the line numbers, and the line is highlighted.

Figure 11.1 shows a breakpoint in the gutter of PriceReport/Program.cs.

![Figure 11.1 - A breakpoint in the gutter](images/ch11-breakpoint.png "width=75%")

*Figure 11.1 - A breakpoint in the gutter*

## Try it

1. Open PriceReport/Program.cs. Put the cursor on the line that declares total, and press {{F9}}.
2. Press {{F5}}. The program runs until it reaches the breakpoint, and stops there.
3. The line with the breakpoint is highlighted in yellow, and a yellow arrow appears in the gutter. The line has not run yet.
4. Press {{Shift+F5}} to stop the program.

## Removing a breakpoint

Press {{F9}} on the same line to remove the breakpoint. Clicking the red dot in the gutter removes it too, which is quicker with the mouse.

## Seeing all breakpoints

The Breakpoints window lists every breakpoint in the solution, with its file and line. Open it with Command Search, and type Breakpoints. Clear a box in the list to disable a breakpoint without removing it.

## Common mistake

A breakpoint on a line that never runs will never be hit. A breakpoint on a blank line or a comment line is also never hit, because nothing runs there. If the program does not stop, check that the breakpoint sits on a line of code.
