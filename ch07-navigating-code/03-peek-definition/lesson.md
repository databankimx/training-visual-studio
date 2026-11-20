# Peek Definition

Go to Definition moves you to another file. Peek Definition shows the definition inside the file you are already working in, so you can read it without losing your place. Put the cursor on a method name, and press {{Alt+F12}}. A box opens under the line with the declaration inside it.

## Try it

1. Open PriceReport/Program.cs and find the line that calls PriceCalculator.MaxPrice.
2. Put the cursor on the word MaxPrice, and press {{Alt+F12}}.
3. Read the declaration in the box that opens. You are still in Program.cs.
4. Press {{Esc}} to close the box.

Figure 7.4 shows Peek Definition on Average. The call sits in PriceReport/Program.cs, and the box shows the declaration in Pricing/PriceCalculator.cs, with the file name at the top.

![Figure 7.4 - Peek Definition on Average, opened from PriceReport/Program.cs](images/ch07-peek-definition.png "width=75%")

*Figure 7.4 - Peek Definition on Average, opened from PriceReport/Program.cs*

## Editing inside a peek

The peek box is a small editor. You can change the code in it, and the change applies to the real file. Use this for a quick fix, and keep larger changes in the file's own window. To open the full file from the peek, click the file name at the top of the box, or press {{F12}}.

## When to use peek and when to use F12

Use Peek Definition when you want to check one definition and then get back to what you were doing. Use Go to Definition when you plan to read or change the file for a while. Both keys start from the same name, so the choice is about how long you will stay.
