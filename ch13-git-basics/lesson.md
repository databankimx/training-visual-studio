# 13. Git Basics in Visual Studio

Git keeps a record of every change you make to a project. Each saved record is a commit, with a message that says what changed and why. You can go back to any commit later, and compare two of them. Visual Studio shows Git through the Git Changes window and the status bar, so most of the work happens without leaving the editor.

## Why source control matters

Source control is the record of how a project got to where it is. Without it, the only copy of your code is the one on your disk, and a mistake can erase it. With it, every change has an author, a time, and a reason, so you can find the commit where a bug first appeared, and undo it without losing the work around it.

It also makes teamwork safe. Other developers can see what you changed before it reaches the main line, and review it, and questions have an answer in the history instead of in someone's memory. At DataBank, custom code must be stored in the company's GitHub Enterprise repository before it is delivered to a client, and reviewed in that repository. A copy on one laptop does not meet that rule, because nobody else can check it, and nobody can support it later.

Good habits start here. Commit small, clear changes, and write messages that a stranger could understand a year from now.

This chapter uses your copy of the practice repository from Chapter 2, on your computer in C:\Development\training-visual-studio-practice. You will make changes, stage them, commit them, and see which branch you are on. A commit stays on your computer until you push it, and Chapter 15 covers pushing.
