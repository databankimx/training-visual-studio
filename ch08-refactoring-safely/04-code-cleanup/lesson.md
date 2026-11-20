# Code Cleanup

Code Cleanup applies a set of fixes to a file in one step. The fixes come from the style rules in the .editorconfig file and from the analyzers that run as you type. Each fix is small on its own, such as removing a using directive that nothing uses, or sorting the using directives into order. Together, they make a file consistent with the rest of the solution.

## Running Code Cleanup

Press {{Ctrl+K}}, then {{Ctrl+E}}, to run Code Cleanup on the current file. Visual Studio applies the fixes at once, and the file is changed, so the tab shows that it has unsaved changes.

Code Cleanup is different from Format Document. Format Document changes only the layout, such as indentation and spacing. Code Cleanup can also change how the code is written, such as removing an unused using directive or applying a style rule.

## Try it

1. Open Pricing/PriceCalculator.cs.
2. Press {{Ctrl+K}}, then {{Ctrl+E}}. Watch the file for any changes.
3. Press {{Ctrl+Z}} to undo the cleanup, and compare the file with its earlier state.

## Common mistake

Code Cleanup works on the file that is open, so run it on one file at a time while you learn it. Check the changes in each file before you save, especially when the file was written before the team settled on its style rules.
