# Creating a branch

Click the branch name in the status bar, at the bottom of the window. The branch menu opens. On the Local tab, choose New Branch. Figure 14.1 shows the menu, with main as the current branch.

![Figure 14.1 - The branch dropdown in the status bar](images/ch14-branch-dropdown.png "width=50%")

*Figure 14.1 - The branch dropdown in the status bar*

Give the branch a name that says what it is for. Use lowercase letters, and join the words with hyphens. A prefix such as feature/ helps you see the kind of work at a glance. For example, feature/document-average describes a change to the Average method. Git does not allow spaces in branch names, so use hyphens instead.

Create the branch. Visual Studio makes the new branch from the commit you are on, and switches to it. The status bar now shows the new name. Every commit you make from here goes onto this branch, and main keeps the commits it already had.

## Try it

1. Click the branch name in the status bar, and choose New Branch on the Local tab.
2. Type feature/document-average, and create the branch.
3. Check that the status bar shows the new name.
