# Reading Git errors

Most Git operations finish quietly. When one fails, Visual Studio tells you in a dialog, and the Output window keeps a record of the steps.

Figure 16.3 shows a failed push. The dialog names the problem: your local branch is behind the remote branch, so you need to pull before you push. It offers three buttons. Pull then Push pulls the waiting commits, and then pushes, in one step. Pull only brings the commits down, so you can look at them first. Cancel leaves everything as it was.

![Figure 16.3 - The push failed dialog](images/ch16-push-failed-dialog.png "width=50%")

*Figure 16.3 - The push failed dialog*

Figure 16.4 shows the Output window with Source Control - Git chosen in its box. It lists the steps of the operation: the commit, then each push attempt. The branch name in the lines is the one you chose, so yours may differ from the figure. It does not repeat the reason for the failure, so read the dialog for that. Open the Output window when a dialog does not explain enough, or when you want to see exactly which branch Git pushed.

![Figure 16.4 - The Output window with Source Control - Git chosen](images/ch16-output-push-lines.png "width=75%")

*Figure 16.4 - The Output window with Source Control - Git chosen*

A second common problem is a sign-in that has expired. Read the dialog to tell the two apart. A rejected push needs a pull, and a sign-in problem needs you to sign in to GitHub again. Read the message before you try a fix.

## Try it

1. Open the Output window from the View menu, and choose Source Control - Git in its box.
2. Find the last few lines of the most recent Git operation, and read them.
3. Close the window, and leave it open if you are going on to the homework.
