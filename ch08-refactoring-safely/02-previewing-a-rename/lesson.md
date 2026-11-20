# Previewing a rename

Before you apply a rename, look at what it will change. The Rename box can show a preview, so you can check every file the rename touches. This matters most for a method used across several projects, where a change in one file is easy to miss.

Figure 8.1 shows the Rename box with its drop-down open, and the preview checkboxes visible.

![Figure 8.1 - The Rename box with the preview options](images/ch08-rename-preview.png "width=75%")

*Figure 8.1 - The Rename box with the preview options*

## Opening the preview

Start the rename as in the last lesson, with {{Ctrl+R}}, then {{Ctrl+R}}. Type the new name. Then open the drop-down at the right side of the Rename box. Checkboxes appear there, and one of them turns on the preview of the changes. Tick the preview, and press {{Enter}}. Visual Studio shows each change in a list, grouped by file, before it saves anything.

## Choosing what the rename updates

The same checkboxes control two other options. One updates comments, and the other updates strings that contain the old name. Turn them on when the name also appears in a comment or a message that should change with it. Leave them off when the word in the comment or string means something else.

## Try it

1. Open Pricing/PriceCalculator.cs and put the cursor on the word Total in its declaration.
2. Press {{Ctrl+R}}, then {{Ctrl+R}}, and type Sum.
3. Open the drop-down in the Rename box, and tick the preview option.
4. Press {{Enter}}. Read the list of changes, and check that the four uses appear: one in PriceCalculator, one in PriceReport, and two in the tests.
5. Press {{Esc}} to stop the rename without changing any file.

## Common mistake

Previewing a rename does not save any change. Once you apply the rename, the files are changed, so use {{Ctrl+Z}} if the result is wrong.
