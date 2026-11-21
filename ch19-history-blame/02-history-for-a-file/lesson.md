# History for one file

The history of the whole repository can be long. Often you want the history of one file, which lists only the commits that changed that file. Right-click the file in the Solution Explorer, or in the editor, and choose Git, then View History. The exact menu may say File History, depending on the version. Figure 19.1 shows the history of Labels.cs, which has several commits from Chapter 17.

![Figure 19.1 - The history view for Labels.cs](images/ch19-file-history.png "width=75%")

*Figure 19.1 - The history view for Labels.cs*

Each row is a commit that touched the file, with its message and date. Select a row to see the change it made to the file, with removed lines in red and added lines in green. Read the change first, and then the message. The message says what the author meant to do, and the change shows what they actually did.

This view is the quickest way to answer, "When did this method start looking like this?" Find the commit that made the change you care about, and read its message and its diff together.

## Try it

1. Right-click Labels.cs, and open its history from the Git menu, or from the context menu.
2. Find the commit with the message Change label to Listed price, from Chapter 17.
3. Select it, and read the change.
