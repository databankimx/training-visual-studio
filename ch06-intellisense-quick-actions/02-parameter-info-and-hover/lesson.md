# Parameter info and hover

Two more features help while you write code. Parameter info shows the parameters a method expects, and it highlights the one you are typing. Hover shows the signature and the type of anything you point at, which saves you from opening the file where it is defined.

## Parameter info

Type the name of a method, followed by an open parenthesis. A small box appears above the line, showing the method's signature. For a method with more than one parameter, the highlighted parameter moves along as you type each comma. If the box closes while you are still typing, press {{Ctrl+Shift+Space}} to bring it back.

Parameter info needs the cursor to be inside the parentheses. If nothing appears, check that you are on the right side of the open parenthesis.

## Hover

Hold the mouse over a name, and a tooltip appears. Over a method, it shows the signature and the return type. Over a variable, it shows the type of the variable. The practice methods use two slashes for their comments, so their tooltips show the signature and the types, which is the information you need here.

Tooltips also show documentation written with three slashes above a method. That documentation is the description other developers read when they hover over your method, so write it for them.

## Try it

1. Open PriceReport/Program.cs. Place the cursor inside the parentheses of the Total call, and read the parameter info box.
2. Hover over the word Total in the call. Read the signature and the return type.
3. Open Pricing/PriceCalculator.cs. Hover over the word prices in the Average method, and read the type it shows.
4. Hover over the word Average in the Average method declaration, and compare the tooltip with the one you saw for Total.
