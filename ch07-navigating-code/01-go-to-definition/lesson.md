# Go to Definition

Go to Definition takes you from a name to the place it is declared. Put the cursor on a method name in a call, press {{F12}}, and Visual Studio opens the file that declares the method, with the cursor on its declaration. You do not have to remember which project or folder holds it.

## Try it

1. Open PriceReport/Program.cs and find the line that calls PriceCalculator.Total.
2. Put the cursor on the word Total in that line, and press {{F12}}.
3. Visual Studio opens Pricing/PriceCalculator.cs, with the cursor on the Total declaration.
4. Press {{Ctrl+-}} to navigate back. The cursor returns to the call in Program.cs.

Navigate Back and Navigate Forward keep a history of where you have been. Press {{Ctrl+-}} to go back, and {{Ctrl+Shift+-}} to go forward again. This history works across files, so you can follow a chain of calls and retrace it.

## The toolbar buttons

The same history is available from the toolbar, as a back arrow and a forward arrow near the left edge. Click the back arrow to go back one step, the same as pressing {{Ctrl+-}}.

Figure 7.1 shows the back and forward arrows on the toolbar, with the forward arrow active.

![Figure 7.1 - The back and forward arrows on the toolbar](images/ch07-toolbar-buttons.png "width=25%")

*Figure 7.1 - The back and forward arrows on the toolbar*

The small arrow beside the back arrow opens a list of recent positions, most recent first. Each entry shows the file and the line where you were. The entry with a check mark is the position you are on now. Choose any entry to jump straight to it, instead of pressing {{Ctrl+-}} several times.

Figure 7.2 shows the list open from the back arrow. The check mark marks the current position.

![Figure 7.2 - The list of recent positions opened from the back arrow](images/ch07-back-dropdown.png "width=75%")

*Figure 7.2 - The list of recent positions opened from the back arrow*

The forward arrow moves one step forward, the same as {{Ctrl+Shift+-}}. It is greyed out when there is nothing to go forward to, and it becomes active once you have gone back. The forward arrow has no list, so use the keyboard shortcut or click it once for each step.

## Go to Definition on a type

The same key works on a type name. Put the cursor on PriceCalculator in Program.cs, and press {{F12}}. The class declaration opens, and you can read the methods it holds from there.

## When the definition is in another project

Go to Definition works across the solution, and across projects that the solution references. The Total method is in the Pricing project, but the call sits in PriceReport, so this example already crosses a project boundary. It is the same key in both cases.

## Common mistake

Go to Definition needs the cursor on the name itself, not on the parenthesis or the space before it. If F12 does nothing, click on the name, then press the key again.
