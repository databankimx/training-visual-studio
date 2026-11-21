# Clean-day checklist

Work through these in order each time you sit down to change code. Change `[ ]` to `[x]` as you go, and save the file. Each step names the chapter that taught it, so you can go back if a step is unclear.

## Open

- [ ] Open the solution in its own Visual Studio window, from the folder you cloned. (Chapter 3)
- [ ] Check the branch name in the status bar, and the Git Changes window. (Chapters 13 and 14)
- [ ] Pull the latest changes if the team shares the branch, and resolve any conflicts before you start. (Chapters 15 and 16)
- [ ] Check the Error List for anything left from yesterday. (Chapter 9)

## Branch

- [ ] Create a branch for the change, with a short name. (Chapter 14)
- [ ] Check the branch name in the status bar before you edit. (Chapter 14)

## Edit

- [ ] Make the change with the editor's tools: Find and Replace, Rename, and IntelliSense. (Chapters 5 to 8)
- [ ] Use Code Cleanup on the file, if your team uses it, and read what it changed. (Chapter 24)
- [ ] Save the file. (Chapter 5)

## Build and test

- [ ] Build the solution, and clear every error in the Error List. (Chapter 9)
- [ ] Run all tests in Test Explorer, and read the expected and actual values for any failure. (Chapter 11)
- [ ] If a test fails, debug it with a breakpoint, and decide whether the code or the test is wrong. (Chapter 12)
- [ ] Run the tests again until they pass for the right reason. (Chapter 25)

## Commit

- [ ] Read every changed line in Git Changes, and unstage anything you did not mean to change. (Chapter 13)
- [ ] Write a clear commit message that says what the change does. (Chapter 13)
- [ ] Commit the staged changes. (Chapter 13)

## Push and review

- [ ] Push the branch, or publish it if it is new. (Chapter 15)
- [ ] Open a pull request, and write a description a reviewer can follow. (Chapter 17)
- [ ] If Copilot explained the code, check the explanation against the code and the tests. (Chapters 19 to 21)
- [ ] Review the pull request's checks and comments before you merge. (Chapter 17)
