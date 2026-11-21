# Renaming a symbol

A symbol is a name in the code, such as a method, a class, or a variable. Renaming a symbol with Visual Studio updates the declaration and every place that uses it, in every file in the solution. Renaming by hand, with Find and Replace, can miss a use or change a word that only looks the same, so use the rename command for names in code.

## Starting a rename

Put the cursor on the name, and press {{Ctrl+R}}, then {{Ctrl+R}}. A small Rename box opens over the name, with the current name selected. Type the new name, and press {{Enter}} to apply it. The name changes at the declaration and in every use.

You can also choose Edit, then Refactor, then Rename, or right-click the name and choose Rename.

## Try it

1. Open Pricing/PriceCalculator.cs and put the cursor on the word Average in its declaration.
2. Press {{Ctrl+R}}, then {{Ctrl+R}}. The Rename box opens.
3. Type Mean, and press {{Enter}}. The declaration changes to Mean.
4. Open PriceReport/Program.cs. The call now reads PriceCalculator.Mean.
5. Press {{Ctrl+Z}} to undo the rename. Check that every file returns to Average.

## A name that already exists

If the new name is already used in the same scope, the Rename box shows a warning and does not apply the change until the conflict is resolved. Read the warning, and choose a different name or rename the other symbol first.

## Common mistake

Renaming a method changes the name everywhere the method is called, including tests. A rename does not change any behavior, so the tests should pass after the rename. If a test fails, check whether the test uses the old name in a string, since a string is not updated unless you ask for it. The next lesson shows how to check the changes before you apply them.
