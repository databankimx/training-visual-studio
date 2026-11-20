# Formatting a document

Formatting fixes the layout of a file: the indentation, the spacing around operators, where braces go, and how lines are broken. Formatting does not change what the code does. Two versions of a method can look very different after formatting and still produce exactly the same answer.

Figure 5.1 shows a method before and after formatting. The code does the same thing in both versions. Only the layout changed.

![Figure 5.1 - A method before and after Format Document](images/ch05-format-before-after.png "width=75%")

*Figure 5.1 - A method before and after Format Document*

## Formatting the whole file

Press {{Ctrl+K}}, then {{Ctrl+D}}. Visual Studio formats the whole file in the editor. The file is changed, so the tab shows that it has unsaved changes. Save it with {{Ctrl+S}} when you are happy with the result.

## Formatting a selection

To format only part of a file, select the lines first. Then choose Edit, Advanced, Format Selection. Use this when a single method was pasted in badly and the rest of the file is already correct.

## Where the rules come from

Formatting follows the style rules in a file named .editorconfig, which sits at the top of the practice repository. The file lists settings such as the number of spaces in an indent and where braces go. Because the rules are in one file, everyone who works on the repository gets the same layout.

## Try it

1. Open Pricing/PriceCalculator.cs.
2. Select the whole file with {{Ctrl+A}}, then press {{Ctrl+K}}, then {{Ctrl+D}}. The lines should now be indented in a consistent way.
3. Look at the indentation inside the Total method, and compare it with the Average method. They should match.
4. Press {{Ctrl+Z}} if you want to see the file change back, or leave it formatted and do not save until you have checked the result.

## Common mistake

Formatting a file that is already in a different style can produce a large set of changes. Look at the diff before you save. If the changes touch lines you did not mean to edit, undo them and format only the selection you need.
