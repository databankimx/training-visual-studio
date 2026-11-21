# Chapter summary

Remember these when a merge conflicts:

- A conflict happens when two branches change the same lines, and Git cannot choose between them.
- The markers show the current branch, which is HEAD, and the incoming branch, separated by an equals line.
- In the merge editor, the checkboxes keep the current text, the incoming text, or both. The Result pane shows the file as it will be saved.
- Resolving is a decision. Commit the merge with a message that says what you chose and why.

```quiz
In a conflict, what does the text between the markers and the equals line come from?
◉ The current branch, which is HEAD
→ Yes. HEAD is the branch you have checked out, such as main.
○ The incoming branch
→ The incoming branch is the text after the equals line.
○ The last commit on GitHub
→ The markers come from the local merge, not from GitHub.
```

```quiz
Which checkbox keeps the text from the branch you merged in?
○ The Current checkbox
→ That keeps the text from your current branch.
◉ The Incoming checkbox
→ Yes. It keeps the text from the branch you merged in.
○ Both checkboxes
→ That keeps both sides, one after the other.
```

```quiz
Why is ticking both checkboxes often a poor choice for a return line?
○ It deletes the commit history.
→ It affects the file, not the history.
◉ It can leave two return statements in a row, so the second one never runs.
→ Yes. The compiler warns about unreachable code, which is a sign the choice needs a second look.
○ It stops the file from being staged.
→ Staging works the same way for every option.
```
