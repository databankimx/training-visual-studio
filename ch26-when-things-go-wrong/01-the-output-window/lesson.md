# The Output window

The Output window shows messages from the parts of Visual Studio that work in the background: builds, debugging, tests, and Git. Open it from the View menu, choose Output, or press {{Ctrl+Alt+O}}.

The Show output from box at the top of the window chooses which source to read. The list depends on what has run recently. Build shows compiler messages, Debug shows the debugger, and Source Control - Git shows the commands Visual Studio ran for Git. When a push fails, the reason often appears in the Git pane, as Chapter 15 showed.

Read the last lines first. The most recent message is usually the one that explains the failure, and the lines above it show what led to it.

## Try it

1. Press {{Ctrl+Alt+O}} to open the Output window.
2. Open the Show output from list, and choose Source Control - Git.
3. Read the last three lines, and note what the most recent one says.
