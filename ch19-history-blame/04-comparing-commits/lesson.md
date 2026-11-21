# Comparing two commits

Sometimes the question is not about one line or one file. It is about everything that changed between two points in the history, such as the start of a feature and its latest commit. Comparing two commits shows every file that differs between them, and the changes in each file.

In the Git Repository window, select one commit, then hold Ctrl and select a second commit. Choose Compare from the menu that appears, or from the right-click menu on the selection. The details pane lists the files that differ between the two commits. Open a file from that list to see the changed lines.

The order matters. Git shows the change from the older commit to the newer one. Added lines are in green, and removed lines are in red, so a comparison that runs the other way looks reversed. Check which commit is older before you read the result.

Comparing two commits is also how you check what a pull request will change. Compare the tip of the feature branch with the tip of main, and you see the same set of changes the pull request shows.

## Try it

1. In the Git Repository window, select the commit for the Chapter 14 comment, and then the most recent commit.
2. Compare them, and read the list of files that differ.
3. Open one file, and check which lines are green and which are red.
