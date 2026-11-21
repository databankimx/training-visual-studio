# Quick Actions

When Visual Studio knows how to fix a problem, it offers a Quick Action. Put the cursor on the underlined text or on the line, and a light bulb appears in the margin. Click the light bulb, or press {{Ctrl+.}}, to open the menu of fixes.

Figure 6.3 shows the Quick Actions menu for a name that is not yet imported.

![Figure 6.3 - The Quick Actions menu with the light bulb](images/ch06-quick-actions.png "width=75%")

*Figure 6.3 - The Quick Actions menu with the light bulb*

## Choosing a fix

Use the arrow keys to move through the menu, and press Enter to apply the highlighted fix. Read the first line of each item before you choose, because the same problem can have more than one fix. Some fixes also offer Preview changes, which shows the edit before Visual Studio applies it.

## Try it

1. Open PriceReport/Program.cs. Click at the end of the line that declares total, and press Enter.
2. Type var builder = new StringBuilder(); on the new line. The name StringBuilder is underlined, because the file has no using directive for it.
3. Press {{Ctrl+.}} with the cursor on StringBuilder. Choose the option that adds the using directive for System.Text.
4. Check the top of the file. A new line reading using System.Text; has been added.
5. Press {{Ctrl+Z}} as many times as needed to return the file to its original state.

## Common mistake

Quick Actions apply a fix at once when you press Enter, so check the menu before you choose. If the result is not what you expected, press {{Ctrl+Z}} to undo it, and try a different option.
