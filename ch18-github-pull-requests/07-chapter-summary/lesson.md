# Chapter summary

Remember these about pull requests:

- A pull request proposes merging one branch into another, and holds the review, the discussion, and the checks in one place.
- Create one on github.com after you push a branch. Give it a title and a description that say what changed and why.
- The Files changed tab shows every changed line. Comment on a line, then submit the review as a comment, an approval, or a request for changes.
- Read the Checks area before you merge, and read a failed check's log.

```quiz
What does a pull request ask for?
○ A copy of the repository on another computer
→ A pull request is not a copy. It proposes merging one branch into another.
◉ A review and merge of one branch into another
→ Yes. The review happens on the pull request before the merge.
○ A new branch with no commits
→ A pull request needs commits on its branch to show a change.
```

```quiz
Where do you leave a comment on one changed line?
◉ The Files changed tab, by clicking the plus sign in the gutter
→ Yes. Hover over the line, click the plus sign, and write the comment.
○ The Output window
→ The Output window shows Visual Studio's messages, not GitHub comments.
○ The Status bar
→ The status bar shows the branch and the arrows, not comments.
```

```quiz
A check on a pull request shows a red X. What should you do?
○ Delete the branch
→ Deleting the branch does not explain the failure.
◉ Open the check's log and read why it failed
→ Yes. The log shows the step that failed, and the reason.
○ Merge the pull request anyway
→ A failed check is a reason to stop and read it first.
```
