# Code Cleanup

Code Cleanup is a set of fixes Visual Studio applies to a file in one step. Depending on the cleanup profile, it can sort the using statements, remove the ones you do not use, and apply the code style rules that the file's settings ask for. It does not change what the code does, but it does change the text, so it shows up in Git.

To run it, open the file, and click the broom button on the file's status bar, at the bottom of the editor. Figure 25.2 shows the menu it opens. The menu lists two cleanup profiles, Profile 1 and Profile 2, and a Configure Code Cleanup command. Choose a profile to run it. The menu shows {{Ctrl+K}} then {{Ctrl+E}} next to Profile 1, so that shortcut runs the first profile.

A profile is a set of cleanup actions. Configure Code Cleanup opens the settings for the profiles. Read what a profile does before you choose it, because the two profiles can do different things.

![Figure 25.2 - The Code Cleanup menu](images/ch25-code-cleanup-menu.png "width=50%")

*Figure 25.2 - The Code Cleanup menu*

Cleanup works on the file that is open. Each change is applied to the text in the editor, so you can press {{Ctrl+Z}} to undo a cleanup you did not want.

The rules come from your settings and from the .editorconfig file in the solution, if there is one. A .editorconfig file is shared with the team when it is committed, so the team sees the same rules. Your choice of profile is saved on your computer.

After cleanup, open Git Changes and read what changed before you commit. A cleanup that touches only the lines you meant to change is a good sign. A cleanup that rewrites a whole file is a reason to check the profile before you go on.

## Try it

1. Open a class in the practice solution, and run Code Cleanup from the broom button on the status bar.
2. Open Git Changes, and read the diff for that file.
3. Press {{Ctrl+Z}} to undo the cleanup if you did not want the change.
