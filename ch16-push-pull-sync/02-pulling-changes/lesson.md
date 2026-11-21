# Pulling changes

A pull brings commits from GitHub into your copy. You need one when a commit lands on the remote branch from somewhere else: a web edit, a commit from another computer, or a change a teammate pushed. Pulling updates your branch and your files to match.

The Git Changes window shows a Pull button with a number beside it. That number is how many commits GitHub has that your branch does not. Click Pull, and the commits come down and your files update.

Pull before you push. If GitHub has a commit you do not have, your push is refused, because pushing would overwrite that commit. Pulling first brings the commit to your computer, so the push can succeed on top of it. The lesson "Reading Git errors" shows the dialog you see in that case.

## Try it

1. On github.com, open your practice repository. Open README.md, and choose Edit. Add one line at the end, and commit it directly to main.
2. Back in Visual Studio, check the Pull button in the Git Changes window. It should show the number 1.
3. Click Pull. Open README.md, and check that the new line is there.
