# Commit the change

A commit saves one step of your work with a message. In Git Changes, stage the one file you changed, and then write the message. Chapter 14 covered staging and committing, so use the same steps.

Write a message that says what the change does, in the present tense. Fix `MinPrice` to return the smallest price is a good message. Fix stuff is not, because a reviewer reads the message before the diff.

Click Commit and Push, if you want the commit to go to GitHub at once, as Chapter 16 showed. The pull request in the next lesson needs the branch on GitHub.

> **Check what you are committing.** Staged files are the ones the commit will include. Read the list before you commit, and make sure it holds only `PriceCalculator.cs`.

## Try it

1. Stage `PriceCalculator.cs` in Git Changes.
2. Write the message Fix `MinPrice` to return the smallest price.
3. Choose Commit and Push, or Commit Staged if you want to push later.
