# Sync and the status bar counts

The status bar at the bottom of the window shows the same information in a compact form. Next to the branch name, arrows show how far your copy has drifted from GitHub. An up arrow with a number means that many commits are waiting to be pushed. A down arrow with a number means that many commits are waiting to be pulled. Figure 16.2 shows the status bar after a commit, with one up arrow beside the branch name.

![Figure 16.2 - The status bar with the ahead count after a commit](images/ch16-status-bar-ahead.png "width=75%")

*Figure 16.2 - The status bar with the ahead count after a commit*

Sync does both steps in one click. It pulls first, then pushes, so the two sides end up matching. The Sync button appears in the Git Changes window once your branch has both incoming and outgoing commits. Click it when you want to reach the same state on both sides, and you do not want to think about the order.

Click the arrows in the status bar to open the Git Changes window, so you can see which commits are on each side before you act.

## Try it

1. Make a small change, and commit it, without pushing.
2. Check the status bar. An up arrow with the number 1 should appear beside the branch name.
3. Click the arrows, and find the commit in the window.
4. Push it, and check that the up arrow disappears.
