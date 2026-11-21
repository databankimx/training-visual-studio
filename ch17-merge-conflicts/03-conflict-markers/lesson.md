# Reading the conflict markers

Open Labels.cs. Git has written both versions of the line into the file, separated by markers. Figure 17.2 shows the section in the editor.

```csharp
public static string PriceLabel(decimal price)
{
<<<<<<< HEAD
    return $"Listed price: {price:C2}";
=======
    return $"Cost: {price:C}";
>>>>>>> feature/label-wording
}
```

![Figure 17.2 - The conflict markers in the editor](images/ch17-conflict-markers.png "width=75%")

*Figure 17.2 - The conflict markers in the editor*

The text between the first marker and the equals line is your current branch, which is main, shown as HEAD. The text between the equals line and the last marker is the branch you merged in. The markers are not valid C#, so the file does not build until you remove them.

Visual Studio also adds a banner at the top of the file: File contains merge conflicts, with an Open Merge Editor link and an Auto Resolve link. The next lesson uses the first link.

Removing the markers is part of resolving the conflict, but it is not the decision. The decision is which text the line should keep. Read both versions, and think about what the program should print.

## Try it

1. Open Labels.cs, and find the three marker lines.
2. Say which version is the current branch, and which is the incoming branch.
3. Do not edit the file yet. The next lesson shows the tools for the change.
