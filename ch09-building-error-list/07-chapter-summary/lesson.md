# Chapter summary

Keep these in mind for the rest of the course:

- Build Solution, with {{Ctrl+Shift+B}}, compiles every project. Ctrl+B builds only the current project, which is faster but can hide a break in another project. Rebuild and Clean are in the Build menu.
- The Error List shows each error and warning with its file and line. The Output window shows the full build log.
- Debug is the default configuration, and Release produces the optimized version.
- Read the errors from the top of the file, and fix the first real one before the others.

```quiz
Which key combination builds the solution?
○ Ctrl+Shift+F
→ Ctrl+Shift+F searches every file for text. Build is Ctrl+Shift+B.
◉ Ctrl+Shift+B
→ Yes. Build Solution compiles every project in the solution.
○ F5
→ F5 runs the program with the debugger. Build Solution is Ctrl+Shift+B.
```

```quiz
Which configuration is the default, and keeps information for the debugger?
◉ Debug
→ Yes. Debug keeps extra information, so you can pause the program and read its values.
○ Release
→ Release optimizes the code, and it leaves out the information the debugger uses.
○ Output
→ Output is a window that shows the build log. It is not a configuration.
```

```quiz
A build reports several errors. Which one should you fix first?
○ The last error in the list
→ The last error is often a result of an earlier mistake, so fixing it first wastes time.
◉ The first real error in the file
→ Yes. Fixing it often removes several of the errors below it.
○ The warning with the highest number
→ Warnings do not stop the build, and the number does not show which one matters most.
```
