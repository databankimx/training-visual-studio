# Blame a line

Blame shows, for each line in a file, the commit that last changed it. It sits beside the code, so you can see the author, the date, and the message next to every line. Blame does not mean fault. It tells you where to look, and the commit message tells you why.

Turn blame on from the Git menu, or from the editor's context menu, and choose the option to annotate or blame the file. Figure 19.2 shows the annotations beside the code of Labels.cs. Each line has a short label with the author and the date. Hover over a label to see the full commit message.

![Figure 19.2 - Blame annotations beside the code in Labels.cs](images/ch19-blame.png "width=75%")

*Figure 19.2 - Blame annotations beside the code in Labels.cs*

Blame answers a narrow question: which commit wrote this line? To see what else that commit changed, select the label and open the commit from the blame view. Then use the history view to read the wider change.

Turn blame off the same way you turned it on when you finish. It stays out of the way of editing, but it covers the window while it is on.

## Try it

1. Turn on blame for Labels.cs.
2. Hover over the label beside the line that returns the price text, and read the commit message.
3. Turn blame off.
