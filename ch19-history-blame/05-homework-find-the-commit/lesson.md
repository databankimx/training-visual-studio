# Homework: find the commit

This exercise has you trace one line back to the commit that wrote it, and read the reason the author gave.

## Work through these steps in order

1. **Pick a line.** In Labels.cs, choose the return line in PriceLabel.
2. **Blame it.** Turn on blame for the file, and find the label beside that line. Write down the author, the date, and the commit message.
3. **Open the commit.** Select the label, and open the commit from the blame view. Read the list of files it changed.
4. **Read the history.** Open the history for Labels.cs, and find the same commit. Count how many commits came before it.
5. **Compare.** Compare that commit with the one before it, and check whether the return line changed in it, and how.

## Check your work

You can name the commit that last changed the total line, its author and date, and the file's history position. You can also say whether the line changed in that commit.

~~~spoiler
Blame reports the last commit that changed the line. The return line may come from the merge you made in Chapter 17, or from one of the two branch commits, depending on how Git recorded the result. Either answer is correct if you can point to the commit and read its message.

If the comparison shows that the line did not change in that commit, the commit still matters, because it may have changed the lines around it. Read the whole change, not only the line you picked.

Turn blame off when you finish.
~~~
