# Chapter summary

Remember these as you share commits:

- Push sends your commits to GitHub. Pull brings commits from GitHub to your computer. Sync does both.
- The status bar arrows show commits waiting to go up or come down.
- A rejected push usually means GitHub has commits you do not have. The dialog offers Pull then Push, or you can pull and push again yourself.
- The Output window, with Source Control - Git chosen, shows the steps of a Git operation.

```quiz
Which button sends your local commits to GitHub?
◉ Push
→ Yes. Push copies your commits to the remote branch.
○ Pull
→ Pull brings commits from GitHub. It does not send yours.
○ Discard Changes
→ Discard Changes removes edits from your files. It does not affect commits.
```

```quiz
A push is rejected. What should you do first?
○ Delete the local branch
→ Deleting the branch would lose your commits.
○ Stash everything and push again
→ Stashing does not add GitHub's commits to your copy.
◉ Pull, then push again
→ Yes. The pull brings in the commits you were missing, and the push can then succeed.
```

```quiz
The status bar shows a down arrow with the number 2 beside the branch name. What does that mean?
○ Two commits are waiting to be pushed to GitHub.
→ That would be an up arrow.
◉ Two commits on GitHub are waiting to be pulled to your computer.
→ Yes. A down arrow counts incoming commits.
○ Two files have uncommitted changes.
→ The arrows count commits, not files.
```
