# Commenting and uncommenting code

A comment is text that Visual Studio ignores when it builds the program. Comments explain what the code is for, and they are also a quick way to switch a block of code off while you test something else. In C#, a comment on a single line starts with two slashes, like this:

```csharp
// This line is ignored when the program runs.
decimal total = 0m;
```

## Commenting out a block

Select the lines you want to switch off. Press {{Ctrl+K}}, then {{Ctrl+C}}. Press the two keys one after the other, not together. Visual Studio adds two slashes at the start of each selected line, and the code stops running. The lines stay in the file, so you can bring them back.

## Uncommenting a block

Select the same lines again. Press {{Ctrl+K}}, then {{Ctrl+U}}. Visual Studio removes the slashes, and the code is live again.

## Toggling with Ctrl+/

Visual Studio also accepts {{Ctrl+/}} for comments, which will feel familiar if you have used Visual Studio Code. Select the lines, and press {{Ctrl+/}} once to comment them out. Press it again on the same lines to remove the comments. Because it is a toggle, one key does both jobs, and you do not need to remember the two-key sequence. Visual Studio added it in version 17.11.

## Using the toolbar

The toolbar also has buttons for commenting and uncommenting the selected lines. Select the lines, then choose the comment button to comment them out, or the uncomment button to remove the comments. Hover over a button to see its name, and the shortcut for it, if it has one.

## Why comment out code

Commenting out is useful while you debug. If a method gives a wrong answer, you can comment out one step to see whether the rest of the method still gives the answer you expect. Commenting out is for short periods, though. Code left in comments for weeks confuses the next person who reads the file, so delete it once you have decided what you want.

## Try it

1. Open Pricing/PriceCalculator.cs. Select the lines of the Total method body, from the line that declares total to the return line.
2. Press {{Ctrl+K}}, then {{Ctrl+C}}. Every selected line now starts with two slashes.
3. Press {{Ctrl+K}}, then {{Ctrl+U}}. The slashes are removed.
4. Press {{Ctrl+/}} to comment the same lines again, then press {{Ctrl+/}} once more to remove the comments.
5. Press {{Ctrl+Z}} if you prefer to undo instead, and check that the file matches the original.
