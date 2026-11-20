# Homework: branch and switch back

This exercise has you create a branch for a single change, commit it there, and check that main is unchanged.

Before you start, commit or stash the change to PriceReport/Program.cs from the Chapter 13 homework, so the working files match the last commit.

## Work through these steps in order

1. **Create a branch.** From the status bar, create feature/document-average from main.
2. **Make the change.** In PriceCalculator.cs, add a comment above the Average method, such as `// Divides the total by the number of prices.`
3. **Commit on the branch.** Stage the file, write a commit message that describes the change, and commit it.
4. **Switch to main.** Click the branch name in the status bar, and choose main.
5. **Check main.** Open PriceCalculator.cs, and confirm the new comment is not there.
6. **Switch back.** Choose feature/document-average, and confirm the comment returns.

## Check your work

The feature branch has one commit more than main. The status bar shows the branch you are on, and the file matches the branch you chose.

~~~spoiler
The comment appears only on feature/document-average, because that is the only branch with the commit. Switching to main takes the file back to its state on main, and switching back restores the commit.

If the switch to main stops with a warning, you have uncommitted changes that would be overwritten. Commit them first, or stash them, and then try the switch again.
~~~
