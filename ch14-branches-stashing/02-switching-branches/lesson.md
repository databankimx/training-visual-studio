# Switching branches

To switch branches, click the branch name in the status bar, and choose the branch you want from the list. Visual Studio checks it out, which means the files on your disk change to match the last commit on that branch.

Try it with the branch from the last lesson. Make a change on feature/document-average, commit it, and then switch to main. The change you committed on the feature branch is gone from the editor, because main does not contain it. Switch back, and it returns. Nothing was lost. The commit lives on the branch, and the branch is just a pointer to it.

Uncommitted changes need care. If the file you have edited is different on the other branch, Visual Studio stops the switch and warns you, so your edits are not overwritten. The safe habit is to commit or stash your changes before you switch.

## Try it

1. On feature/document-average, add a comment to PriceCalculator.cs, and commit it.
2. Click the branch name in the status bar, and choose main.
3. Open PriceCalculator.cs, and check that the comment is not there.
4. Switch back to feature/document-average, and check that the comment returns.
