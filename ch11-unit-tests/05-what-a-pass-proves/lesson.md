# What a passing test proves

A green check mark means one thing: for the inputs in that test, the method returned the value the test expected. It does not mean the method is correct for every input, and it does not mean the test checks anything useful.

Consider a version of Average that takes a shortcut. Imagine someone changes it to this:

```csharp
public static decimal Average(IReadOnlyList<decimal> prices)
{
    return Total(prices) / 2m;
}
```

The method now divides by 2, no matter how many prices there are. Run the test Average_OfTwoAndFour_IsThree. The total of 2 and 4 is 6, and 6 divided by 2 is 3. The test passes, and the bug is still there.

The test passes because two prices and a divisor of 2 happen to give the right answer. Try the same shortcut with three prices, 1, 2, and 3. The average is 2, but the shortcut returns 3. A test with those three prices would fail, and it would show the bug.

This is why a good test suite uses inputs that differ from one another, and includes the edge cases: an empty list, a list with one price, and a list where every price is the same. Each edge case catches a different kind of mistake.

A passing test can also hide a mistake in its expected value. If you copy the expected number from the program's output without working it out, the test agrees with the bug. Work out the answer by hand before you run the test.

## Try it

Do not change the practice project for this lesson. Work through the example on paper. Write down the result of Average on the list 1, 2, and 3, using the correct method. Then write down what the shortcut returns, and check your answer against the paragraph above.
