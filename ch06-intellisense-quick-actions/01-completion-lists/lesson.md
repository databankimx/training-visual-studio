# Completion lists

When you type a dot after a name, Visual Studio opens a completion list. The list holds everything that name offers, such as the methods and properties of a class. Start typing a name, and the list narrows to match what you have typed so far. Press Tab or Enter to insert the item that is highlighted.

Figure 6.1 shows a completion list after a dot.

![Figure 6.1 - A completion list after a dot](images/ch06-completion-list.png "width=40%")

*Figure 6.1 - A completion list after a dot*

Each item has an icon that tells you what kind of member it is. A method, a property, and a class each have their own icon, so you can tell them apart before you pick one.

## Try it

1. Open PriceReport/Program.cs. Click at the end of the line that declares total, and press Enter to start a new line.
2. Type PriceCalculator and then a dot. The completion list opens with the members of PriceCalculator.
3. Type Av. The list narrows to Average.
4. Press Tab. Visual Studio inserts Average at the cursor.
5. Press {{Ctrl+Z}} to remove the line, so the file is back to its original state.

## Bringing the list back

If the list closes before you pick an item, press {{Ctrl+Space}} to open it again at the cursor. This works anywhere you are typing a name, even if you did not type a dot first.

## Closing the list

Press {{Esc}} to close the list without inserting anything. This matters when you have pressed Enter by mistake. Enter inserts the highlighted item, and the code you meant to type on a new line is replaced by the item. Press {{Esc}} first when you are not sure which item is highlighted.
