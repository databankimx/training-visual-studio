# Homework: push, pull, and sync

This exercise creates the situation from the lesson "Reading Git errors", so you can see the error and fix it.

## Work through these steps in order

1. **Make a local commit.** In your copy, add a comment to PriceCalculator.cs above the Total method, and commit it on main. Do not push yet.
2. **Make a remote commit.** On github.com, edit README.md, and commit the change directly to main.
3. **Try to push.** Click Push in the Git Changes window. The push should be rejected, and a dialog should appear.
4. **Read the dialog.** Find the reason for the rejection, and open the Output window with Source Control - Git chosen to see the steps.
5. **Pull.** Click Pull. Visual Studio brings the website commit to your computer. Your local commit may need a merge if both sides changed the same lines; this exercise avoids that, because the changes are in different files.
6. **Push again.** Click Push. The status bar should show no arrows beside the branch name.

## Check your work

Both commits, yours and the website's, are in the history on GitHub, and the status bar shows no up or down arrows.

~~~spoiler
The push was rejected because GitHub had the README commit, and your copy did not. Pulling brought it down, so your branch was no longer behind. Pushing then added your commit on top of it.

Because the two commits changed different files, Git combined them with no conflict. Chapter 17 covers what happens when both sides change the same lines.
~~~
