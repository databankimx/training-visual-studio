# Chapter summary

Remember these when you need to know where a change came from:

- The Git Repository window shows the history of the repository, newest first.
- The file history shows only the commits that changed one file. Read each commit's message with its change.
- Blame shows the commit that last changed each line. Use it to find where to look, then read the commit.
- Compare two commits to see every file that differs between them, and check which one is older.

```quiz
Which view shows the commit that last changed each line of a file?
○ The Git Repository window
→ The Git Repository window lists commits, not the commit behind each line.
○ The file history
→ The file history lists every commit that changed the file, not the last one for each line.
◉ Blame
→ Yes. Blame puts the author and commit beside each line.
```

```quiz
You want the commits that changed one file. Which view do you open?
◉ The file history, from the Git menu or the right-click menu
→ Yes. It lists only the commits that changed that file.
○ Blame, on the whole solution
→ Blame works on one file at a time, and shows the last change to each line.
○ The Output window
→ The Output window shows messages from Visual Studio, not the history.
```

```quiz
In a comparison of two commits, why does the order matter?
○ It does not matter, because the changes are the same either way.
→ The colors and direction of the changes reverse if you swap the commits.
◉ Git shows the change from the older commit to the newer one, so swapping them reverses the result.
→ Yes. Check which commit is older before you read the green and red lines.
○ It only matters for the first commit in the history.
→ The order matters for any two commits, not only the first.
```
