# Starting a program

There are two ways to run the startup project, and they differ in whether the debugger is attached. Press {{F5}} to start with the debugger. Press {{Ctrl+F5}} to start without it.

With the debugger attached, the program runs until it reaches a breakpoint, which you will set in the next lesson, or until it finishes. Without the debugger, the program runs at full speed and you cannot pause it. Use Ctrl+F5 when you only want to see the output, and F5 when you plan to look inside the program.

## Try it

1. Press {{F5}} to start PriceReport. The program runs to the end, and the Console window prints the four results.
2. Press {{Ctrl+F5}}. The Console window prints the same results, and then shows a message asking you to press any key before it closes.
3. Press any key to close the Console window.
4. Press {{F5}} again, and watch the toolbar. The debug toolbar shows the controls for a running program.

## Stopping a program

Press {{Shift+F5}} to stop a program that is running under the debugger. Visual Studio ends the program and returns to editing. Use the stop button on the debug toolbar if you prefer the mouse.

## Restarting

Press {{Ctrl+Shift+F5}} to restart the program. It stops the current run and starts again, which saves you from stopping and then starting. Restart is useful after you change a line and want to see the change without a full stop.

## Common mistake

A console program with no breakpoints finishes quickly under F5, and the Console window closes before you can read it. Use Ctrl+F5 to keep the window open, or add a breakpoint, which the next lesson covers.
