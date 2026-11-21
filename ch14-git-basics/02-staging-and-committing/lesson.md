# Staging and committing

Git works in three steps. You change files. You stage the files you want in the next commit. Then you commit the staged files with a message. Staging lets you choose which changes belong together, so one commit can hold one idea, even when you have edited several files.

To stage a file, hover over its name in the Changes list, and click the plus sign that appears. The file moves into Staged Changes. Figure 14.1 shows one file staged, with its name in the lower list and the commit box above the lists.

![Figure 14.1 - The Git Changes window with one file staged and the commit box](images/ch14-git-changes-staged.png "width=50%")

*Figure 14.1 - The Git Changes window with one file staged and the commit box*

Click in the commit box, and type a message. A good message has a short first line that says what the commit does, in the present tense, such as Add a comment to the report. Leave a blank line after it if you want to add more detail below. Then click Commit Staged.

Git stamps the commit with your name and the noreply address you set in Chapter 2. The commit goes into the history on your computer. It is not on GitHub yet, and the Git Changes window now shows the commit at the top of its history list.

## Try it

1. Hover over Program.cs in the Changes list, and click the plus sign to stage it.
2. Type Add a comment to the report in the commit box.
3. Click Commit Staged, and check that the Changes list is empty.
