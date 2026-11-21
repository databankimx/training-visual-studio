# Pushing your commits

A commit you have made on your computer is not on GitHub until you push it. Push sends the commits your branch has that GitHub does not, and adds them to the remote copy of the branch.

After you commit, the Git Changes window shows a Push button, with a number beside it. The number is how many commits are waiting to go up. Figure 15.1 shows the window with the Push button and that count. Click Push, and wait for the operation to finish. The count goes back to zero.

![Figure 15.1 - The Git Changes window with the Push button and the outgoing count](images/ch15-git-changes-push.png "width=50%")

*Figure 15.1 - The Git Changes window with the Push button and the outgoing count*

## Commit and push in one step

Separating the commit from the push is useful when you are learning, but in daily work most people finish a commit and send it straight away. The commit button has a dropdown beside it. Choose Commit and Push to commit the staged files and push them in one click, or Commit and Sync to commit, pull any waiting commits, and then push. You will use one of these most of the time. The steps above show each part on its own so you can see what each one does.

If your branch has never been on GitHub before, Visual Studio offers to publish it instead. Publishing does the same job as a first push, and it tells GitHub to track the branch from then on. Accept the prompt for main in your practice repository.

Pushing does not change your files. It only copies commits. Your working files stay as they are.

## Try it

1. In the Git Changes window, find the Push button and the number beside it.
2. Click Push, and wait for it to finish.
3. Open your practice repository on github.com, and check that the commits from Chapters 13 and 14 are in its history.
