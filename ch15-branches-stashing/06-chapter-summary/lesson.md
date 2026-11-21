# Chapter summary

Remember these as you work with branches:

- A branch is a separate line of commits. New commits go onto the branch you are on.
- Switch branches from the branch dropdown in the status bar. The files change to match the branch.
- Commit or stash before you switch, so your edits are not overwritten.
- A stash sets aside uncommitted changes. Apply it later to bring them back.

```quiz
Where do you switch to another branch?
◉ The branch dropdown in the status bar
→ Yes. Click the branch name, and choose the branch from the list.
○ The Solution Explorer
→ The Solution Explorer shows projects and files, not branches.
○ The Test Explorer
→ The Test Explorer shows test results.
```

```quiz
What does a stash do?
○ It deletes your changes for good.
→ A stash keeps the changes. It does not delete them.
○ It commits your changes to GitHub.
→ Stashing does not commit, and nothing goes to GitHub.
◉ It sets your uncommitted changes aside, and leaves the files matching the last commit.
→ Yes. You can apply the stash later to bring the changes back.
```

```quiz
Which branch name follows the advice in this chapter?
○ my stuff
→ Git does not allow spaces in branch names.
◉ feature/document-average
→ Yes. It is lowercase, uses hyphens, and has a prefix that shows the kind of work.
○ FIX THE THING NOW
→ Capital letters and spaces make a name hard to read and type. Use lowercase words joined with hyphens.
```
