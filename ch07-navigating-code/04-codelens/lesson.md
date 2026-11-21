# CodeLens reference counts

CodeLens shows small pieces of information above a declaration, in a dimmer font. The most useful one for navigation is the reference count, which tells you how many places use the method, type, or property. You see it without searching or pressing a key.

Figure 7.5 shows the CodeLens line above the Total method. It reads 4 references, which matches the four results in Figure 7.3.

![Figure 7.5 - The CodeLens reference count above Total](images/ch07-codelens.png "width=75%")

*Figure 7.5 - The CodeLens reference count above Total*

## Opening the references

Click the reference count, and Visual Studio opens the references in a box inside the editor, grouped by file, with each use shown on its line. The box holds the same results as Find All References, so clicking the count is an alternative to pressing {{Shift+F12}}.

Use the count when you want to see the callers while you keep reading the declaration. Use {{Shift+F12}} when you want the full results window, which stays open while you move through the list.

## Reading the count

A count of 0 on a public method can mean the method is unused, or that other code outside the solution calls it. A count that changes as you work tells you the code is being used more or less than before. Treat the number as a hint to look, and use Find All References when you need the full list.

## Try it

1. Open Pricing/PriceCalculator.cs and find the line above the Total declaration.
2. Read the count, and compare it with the four results in Figure 7.3.
3. Click the count. The references list opens. Double-click one result to go to its line.
