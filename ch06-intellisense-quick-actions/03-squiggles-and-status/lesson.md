# Squiggles and the status bar

As you type, Visual Studio checks the code in the background. When it finds a problem, it underlines the problem. A red wavy line is an error, which means the code will not build as written. Other colors mark warnings and suggestions, which may still build. Hover over an underline to read the message, and the message names the problem.

The status bar at the bottom of the editor summarizes the file. When the file has no problems, it reads No issues found, as it did in the status bar you saw in Chapter 0. When there are problems, the status bar shows the number of errors and warnings instead.

Figure 6.2 shows the three kinds of marks Visual Studio uses: an error, a warning, and a suggestion.

![Figure 6.2 - An error, a warning, and a suggestion in one file](images/ch06-squiggles.png "width=75%")

*Figure 6.2 - An error, a warning, and a suggestion in one file*

## The Error List

The Error List window lists every error and warning in the solution, not just the file you have open. Open it with Command Search, using {{Ctrl+Q}}, and type Error List. Double-click an item in the list to go to the line that has the problem.

## Try it

1. Open PriceReport/Program.cs. Click at the end of the line that declares total, and press Enter.
2. Type int count = "five"; on the new line. A red wavy line appears under the text "five".
3. Hover over the underline. Read the message. It names both the type the value is and the type the variable expects.
4. Open the Error List with Command Search. Find the error, and double-click it. The cursor moves to the line.
5. Press {{Ctrl+Z}} to remove the line, and check that the underline disappears.

## Common mistake

A single typo can produce several underlines, because the code that follows depends on the broken line. Fix the first underline in the file, and check whether the others disappear before you fix them one by one.
