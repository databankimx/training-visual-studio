# Stepping through code

When the debugger is paused, you can move through the program one step at a time. Each key does one job, and the difference matters most when a line calls a method.

- **Step Over, with {{F10}}:** runs the current line, and pauses at the next line. If the line calls a method, the method runs in full, and you do not see inside it.
- **Step Into, with {{F11}}:** runs the current line, and if it calls a method, pauses at the first line of that method.
- **Step Out, with {{Shift+F11}}:** runs the rest of the current method, and pauses at the line after the call that brought you into it.
- **Continue, with {{F5}}:** runs until the next breakpoint, or until the program ends.

## Try it

1. Open PriceReport/Program.cs, and set a breakpoint on the line that declares total with {{F9}}.
2. Press {{F5}}. The program pauses on that line.
3. Press {{F11}}. The debugger moves into PriceCalculator.Total in Pricing/PriceCalculator.cs, and pauses at its first line.
4. Press {{F10}} several times. Each press moves to the next line in the method, and the loop runs once for each price.
5. Press {{Shift+F11}} to leave Total. The debugger returns to the line in Program.cs that called it.
6. Press {{F5}} to continue to the end.

## Common mistake

Pressing F11 on a line that calls a framework method, such as Console.WriteLine, can take you into code you did not write. Use F10 on those lines, or Shift+F11 to leave, so you stay in your own code.
