# The merge editor

The conflict markers show what Git could not combine. The merge editor is the easier place to decide. Click Open Merge Editor in the banner at the top of the file. Figure 17.3 shows the editor.

![Figure 17.3 - The merge editor with the incoming, current, and result panes](images/ch17-merge-editor.png "width=75%")

*Figure 17.3 - The merge editor with the incoming, current, and result panes*

The editor has three panes. The Incoming pane on the left shows feature/label-wording, and the Current pane on the right shows main. The Result pane at the bottom is the file as it will be saved. Each conflict has a checkbox at the start of its line, in the Incoming and Current panes:

- Tick the Incoming checkbox to take the line from feature/label-wording.
- Tick the Current checkbox to take the line from main.
- Tick both checkboxes to keep both lines, one after the other.

The Result pane may first show the line that both branches started from, which is the version from "Setting up the conflict", committed before either branch changed it. In Figure 17.3 that line is Price: {price:C}. It is neither of the two choices, so tick a checkbox to replace it with one of the lines from the panes above. You can also type a different line into the Result pane, as long as the file builds.

The bar at the top shows how many conflicts remain, with arrows to move between them. Auto Resolve lets Visual Studio choose the result for you, which skips the decision this chapter teaches, so do not use it here.

When the Result pane shows the line you want, click Accept Merge to save the file. The conflict is then resolved in the file, and the merge is ready to commit. Stage Labels.cs in the Git Changes window, and commit the merge.

## Try it

1. Click Open Merge Editor in the banner at the top of Labels.cs.
2. Find the Incoming, Current, and Result panes, and the count of conflicts at the top.
3. Close the editor without accepting the merge, and leave the conflict in place for the homework.
