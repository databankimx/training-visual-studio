# Open the practice repository

Before you touch anything, look. A red test is often caused by leftover changes, and a lot of wasted time begins with someone editing the wrong copy of the code.

Open the practice solution from your clone of the practice repository, which you made in Chapter 2. Use File, Open, and Project/Solution, and choose `PracticeSolution.sln`. If Visual Studio already shows a different solution, open this one in a new window, so your other work stays where it is.

Next, check the branch. The branch name shows in the status bar at the bottom of the window. It should be main. Open the Git Changes window, and check that the list is empty. If there are changes, read each one before you do anything else. A change you do not recognize is a question to answer first, not a file to commit.

## Why check first

If you start a branch with leftover changes, those changes come along for the ride. They end up in your commit without you choosing them, and a reviewer has to work out why they are there.

> **Check before you branch.** The solution is open, the branch is main, and Git Changes is empty. Those three facts are the starting point for everything in this chapter.

## Try it

1. Open `PracticeSolution.sln` from your clone of the practice repository.
2. Read the branch name in the status bar, and check it says main.
3. Open Git Changes, and confirm there are no changes listed.
