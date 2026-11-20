# Homework: stage one change

This exercise has you make two separate changes, and commit only one of them. The point is to see that staging chooses what goes into a commit.

## Work through these steps in order

1. **Change PriceCalculator.cs.** Add a comment line above the Average method, such as `// The average price. An empty list has an average of 0.` The file already has comments like this, so match their style.
2. **Change Program.cs.** In PriceReport, add a comment line above the line that reads `decimal total`, such as `// Total of the prices above.`
3. **Look at the Changes list.** Both files should appear there. Double-click each one, and check the change.
4. **Stage one file.** Stage PriceCalculator.cs only.
5. **Commit it.** Write a commit message that says what the change does, such as Document the Average method. Click Commit Staged.
6. **Check the window.** Program.cs should still be in the Changes list, and the commit should be at the top of the history.

## Check your work

Your history has one new commit, and Program.cs is still an unstaged change.

~~~spoiler
Only PriceCalculator.cs went into the commit, because it was the only file you staged. The Changes list still shows Program.cs, so you can stage and commit it as a separate commit with its own message.

The commit message should describe the change in one line. Document the Average method is a good example, while update files says nothing about what changed. Keeping one idea in each commit makes the history easier to read later, and easier to undo one part of.
~~~
