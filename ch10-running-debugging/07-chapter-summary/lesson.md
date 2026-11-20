# Chapter summary

Remember these as you debug:

- {{F5}} starts with the debugger, and {{Ctrl+F5}} starts without it. {{Shift+F5}} stops the program.
- {{F9}} sets a breakpoint, and the program pauses there when run under the debugger.
- {{F10}} steps over a line, {{F11}} steps into a method, and {{Shift+F11}} steps out of one.
- The Locals window shows variables, the Watch window follows expressions you choose, and the Immediate window runs code while the program is paused.

```quiz
Which key starts the program with the debugger attached?
○ Ctrl+F5
→ Ctrl+F5 starts the program without the debugger, so breakpoints do not pause it.
◉ F5
→ Yes. The program runs until it reaches a breakpoint, or until it finishes.
○ F9
→ F9 sets or removes a breakpoint. It does not start the program.
```

```quiz
You are paused on a line that calls a method. Which key moves you into that method?
○ F10
→ F10 runs the whole call, and pauses at the next line in the current method.
◉ F11
→ Yes. Step Into pauses at the first line of the method being called.
○ Shift+F11
→ Shift+F11 leaves the current method, and pauses after the call that brought you into it.
```

```quiz
Which window lets you evaluate code while the program is paused?
○ Locals
→ The Locals window lists the variables in the current method.
○ Watch
→ The Watch window follows the expressions you add. It does not run new code.
◉ Immediate
→ Yes. Type an expression in the Immediate window, and press Enter to see its value.
```
