# Cleanup on save

You can ask Visual Studio to run Code Cleanup every time you save a C# file. That is convenient, and it is also a reason to be careful. The cleanup runs on every save, so every save can change the text of a file.

To turn it on, open the Tools menu, choose Options, and select Text Editor in the tree. Find the setting named Select a Code Cleanup profile to run on save. Choose the profile in its list. On this computer the setting shows Profile 1, and the Configure Code Cleanup button beside it opens the profile settings. Make sure your team uses the same profile.

Figure 24.3 shows the setting in the Options window.

![Figure 24.3 - The cleanup on save setting in Text Editor](images/ch24-cleanup-on-save-option.png "width=75%")

*Figure 24.3 - The cleanup on save setting in Text Editor*

Cleanup on save only runs on the files you save. It does not change files you have not opened.

Use it with two habits. First, keep your team's shared .editorconfig file as the source of the rules, so that cleanup on your computer matches what your teammates get. Second, check Git Changes before you commit, and look for any change you did not make on purpose.

If a save produces a surprising diff, undo it with {{Ctrl+Z}}, and check the profile before you save again.

## Try it

1. Open Options, and select Text Editor in the tree.
2. Read the label Select a Code Cleanup profile to run on save, and note the profile it shows. Do not change it yet.
3. Choose Cancel to close the dialog without changes.
