# Homework: follow the references

This exercise asks you to follow one method through the solution with the navigation keys from this chapter. You do not change any code. You only read it, and you report what you find.

## The questions

Answer these three questions about PriceCalculator.MaxPrice:

1. How many references does MaxPrice have? Use CodeLens, then check the count with Find All References.
2. Which two files use it? Write down both file names.
3. In the file that calls MaxPrice inside a test, what is the value the test expects?

## Steps to follow

1. Open Pricing/PriceCalculator.cs. Put the cursor on the word MaxPrice in its declaration, and press {{Shift+F12}}. Count the results.
2. Double-click the result in PriceReport/Program.cs. The file opens at the call.
3. Put the cursor on MaxPrice in that call, and press {{F12}}. The declaration opens.
4. Press {{Ctrl+-}} to go back to the call, then {{Ctrl+-}} again to go back to the results.
5. Double-click the result in Pricing.Tests/PriceCalculatorTests.cs, and read the test. The expected value is written in the Assert line.

## Check your answers

When you have finished, compare your answers with the worked solution below.

~~~spoiler
1. `MaxPrice` has 2 references. CodeLens shows 2 references above the declaration, and Find All References lists the same two results.
2. The two files are `PriceReport`/`Program.cs` and `Pricing.Tests`/`PriceCalculatorTests.cs`.
3. The test calls `MaxPrice` with the values 1.5, 9, and 3, and expects 9 as the answer. Check the Assert line in the test to confirm the expected value.

Going back with {{Ctrl+-}} takes you through each step in the order you visited it, so you can retrace the path without searching again.
~~~
