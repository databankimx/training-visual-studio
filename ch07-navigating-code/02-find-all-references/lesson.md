# Find All References

Find All References lists every place a name is used in the solution. Put the cursor on a method, a type, or a variable, and press {{Shift+F12}}. The results appear in a window, grouped by file, with each use shown on its line.

Figure 7.3 shows the results for PriceCalculator.Total. It lists four uses: one inside Average, one in PriceReport, and two in the test project.

![Figure 7.3 - Find All References results for Total](images/ch07-find-all-references.png "width=75%")

*Figure 7.3 - Find All References results for Total*

## Try it

1. Open Pricing/PriceCalculator.cs, and put the cursor on the word Total in the method declaration.
2. Press {{Shift+F12}}. Count the results, and check that there are four.
3. Double-click the result in Pricing.Tests/PriceCalculatorTests.cs. The file opens at that line.
4. Press {{Ctrl+-}} to navigate back to the results, or back to PriceCalculator.cs.

## Why it matters before a change

Before you rename a method or change what it returns, look at every place that calls it. Find All References tells you which callers will be affected. A method with two callers needs two checks. A method with forty callers needs a plan.

## Common mistake

Find All References follows the name, so a result can be a different method with the same name in another class. Read the file name and the line before you assume a result is the one you wanted.
