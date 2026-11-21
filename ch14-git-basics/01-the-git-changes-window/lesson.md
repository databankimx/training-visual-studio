# The Git Changes window

Open the practice solution in Visual Studio, and make a change first. In Program.cs in PriceReport, add this line above the first Console.WriteLine:

```csharp
// Prices for the report, in dollars.
```

Save the file. Nothing in Git has changed yet. Git only records a change when you commit it, but Visual Studio notices the edit straight away.

Open the Git Changes window from the View menu. Choose Git Changes. Figure 14.1 shows the window with the changed file listed under Changes. The window has two lists. Changes holds files that Git sees as edited, and Staged Changes holds the files you have picked for the next commit.

Double-click Program.cs in the Changes list. Visual Studio opens a view that shows the old and new text side by side, with the line you added highlighted. Read this view before you commit. It is the last check on what you are about to record.

## Try it

1. Add the comment line to PriceReport/Program.cs, and save the file.
2. Open the Git Changes window from the View menu.
3. Double-click Program.cs in the Changes list, and find the line you added.
