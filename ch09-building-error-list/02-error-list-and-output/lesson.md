# The Error List and the Output window

Two windows report what a build did. The Error List shows each error and warning as a row, with the file, the line, and a code such as CS0103. The Output window shows the full log of the build, project by project, in the order the compiler worked through them.

Figure 9.1 shows the Error List after a build with an error in it.

![Figure 9.1 - The Error List with a build error](images/ch09-error-list.png "width=60%")

*Figure 9.1 - The Error List with a build error*

## The Error List

Open the Error List with Command Search, using {{Ctrl+Q}}, and type Error List. Each row has an icon for its severity, the text of the message, the file and line, and the project. Double-click a row to open the file at that line.

The buttons above the list show a count for each kind of row, such as 1 Error and 0 Warnings. Click one to show only those rows. The Messages button shows information from the build. The Entire Solution dropdown on the left sets which files the list covers.

## The Output window

Open the Output window with Command Search, and type Output. Use the Show output from list to choose Build. The window shows each project as it builds, along with the compiler's command and result. Use it when the Error List is empty but the build still failed, or when you want to see which project a message came from.

Figure 9.2 shows the Output window after the same failed build. The last lines count the projects that succeeded, failed, or were up to date.

![Figure 9.2 - The Output window after a failed build](images/ch09-output-window.png "width=75%")

*Figure 9.2 - The Output window after a failed build*

## Try it

1. Open PriceReport/Program.cs. At the end of the line that prints the total, add a new line that reads `int count = "five";`, and save the file.
2. Press {{Ctrl+Shift+B}}. The build fails.
3. Open the Error List. Double-click the row for the error. The cursor moves to the line you added.
4. Press {{Ctrl+Z}} to remove the line, and save the file.

## Common mistake

Errors in a list can come from a single mistake. A missing semicolon often produces a second error on the next line, so the first row is the one to fix. The next lesson shows how to read the list in order.
