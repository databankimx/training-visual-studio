# The Test menu

Visual Studio gathers its test commands under one menu, named Test. You will find it in the menu bar, with File, Edit, and the others. Figure 12.1 shows the menu open. Each command has its keyboard shortcut written to the right of its name.

![Figure 12.1 - The Test menu with its keyboard shortcuts](images/ch12-test-menu.png "width=50%")

*Figure 12.1 - The Test menu with its keyboard shortcuts*

Many shortcuts in this menu have two parts, such as Ctrl+R, A. That means you press Ctrl and R together, let go, and then press A. Visual Studio uses this pattern for groups of related commands, so Ctrl+R is the start of every run command.

## Running tests

- **Run All Tests** (Ctrl+R, A) runs every test in the solution.
- **Repeat Last Run** (Ctrl+R, L) runs the same tests as the last time. It is grayed out until you have run something.
- **Debug All Tests** (Ctrl+R, Ctrl+A) runs every test with the debugger attached, so breakpoints can pause them. Chapter 13 uses it.
- **Debug Last Run** (Ctrl+R, D) does the same for the last run.
- **Clear All Test Results** (Ctrl+R, Del) removes the pass and fail marks, so the tests show as not run.

## Windows and results

- **Test Explorer** (Ctrl+E, T) opens the window where you see every test and its result. You will use it in the next lesson.
- **Code Coverage Results** (Ctrl+E, C) shows the results of a coverage run, which records the lines the tests reach. Analyze Code Coverage for All Tests starts that run.

## Settings and sound

- **Play a Sound When Tests Finish Running** (Ctrl+R, S) plays a sound when a run ends, which helps when a long run finishes while you are away from the screen.
- **Configure Run Settings**, **Configure Remote Test Environments**, and **Processor Architecture for AnyCPU Projects** control how tests run. The defaults suit the practice solution, so you can leave them alone for now.
- **Options** opens the Options dialog.

## Try it

1. Click Test in the menu bar, and find Run All Tests and its shortcut, Ctrl+R, A.
2. Press {{Ctrl+E}}, then {{T}}. Test Explorer opens.
3. Press {{Ctrl+R}}, then {{A}}. Every test runs, and Test Explorer shows the results.
