# Homework: fix the code

This is the homework for the chapter. Fix `MinPrice` yourself, then run the tests and check the result. You have the evidence from the last two lessons, so you do not need a hint. Do not read the spoiler until you have tried.

## Work through these steps in order

1. **Find the line.** Open `PriceCalculator.cs`, and find the return line in `MinPrice`.
2. **Change it.** Make the method return the smallest price, not the largest.
3. **Save the file.** Press {{Ctrl+S}}.
4. **Run all tests.** Press {{Ctrl+R}} then {{A}}, and check that every test passes.
5. **Check the diff.** Open Git Changes, and read the change. It should touch the one line, and nothing else.

## Check your work

Every test in Test Explorer passes, and Git Changes shows one changed line in `PriceCalculator.cs`.

~~~spoiler
Change `prices.Max()` to `prices.Min()` in `MinPrice`. The test expects 1.5, and `Min` of 1.5, 9, and 3 is 1.5.

If Git Changes shows more than one line, check that Visual Studio did not reformat the file. Code Cleanup in Chapter 24 can change text you did not mean to change, so undo it if it did.

If a test still fails, read its message again. It tells you which input, and which answer it got.
~~~
