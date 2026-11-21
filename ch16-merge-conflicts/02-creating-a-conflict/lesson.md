# Creating a conflict

Create a branch named feature/label-wording from main. Using the branch dropdown in the status bar, choose New Branch on the Local tab, as in Chapter 14.

On that branch, change the return line in Labels.cs to this, and commit it with the message Change label to Cost:

```csharp
return $"Cost: {price:C}";
```

Switch back to main, using the branch dropdown. Change the same return line to this, and commit it with the message Change label to Listed price:

```csharp
return $"Listed price: {price:C2}";
```

Both branches now have a different version of the same line, and neither branch has the other's change. Now merge feature/label-wording into main. Make sure main is the checked-out branch, then open the merge dialog from the Git menu, using Manage Branches, and right-click feature/label-wording to start the merge into main. Figure 16.1 shows the dialog.

![Figure 16.1 - The Merge branches dialog with one file that may conflict](images/ch16-merge-dialog.png "width=50%")

*Figure 16.1 - The Merge branches dialog with one file that may conflict*

Read the dialog from top to bottom:

- **Merge into 'main'** names the branch that receives the changes. It is the branch you have checked out.
- **The dropdown** picks the branch to bring in. It already shows feature/label-wording, because you started the merge from that branch. Leave it as it is.
- **The list** shows the files Git expects to conflict. Here it is Labels.cs, the one line you changed on both branches.
- **Merge Manually** starts the merge and leaves the conflict for you to resolve. Choose this button for this chapter.
- **Auto Resolve** lets Visual Studio choose the result for you. That skips the decision this chapter teaches, so do not use it here.
- **Cancel** closes the dialog without merging anything.

The checkbox above the buttons commits a merge automatically, but only when there are no conflicts. Your merge has a conflict, so the checkbox has no effect here. Leave it as it is.

Choose Merge Manually. The Git Changes window now shows Labels.cs under a Conflicts heading.

## Try it

1. Create feature/label-wording from main, change the return line, and commit.
2. Switch to main, change the same line differently, and commit.
3. Open the merge dialog, choose Merge Manually, and check that Labels.cs is listed as a conflict.
