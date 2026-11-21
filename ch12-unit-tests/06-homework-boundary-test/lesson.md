# Homework: add a boundary test

This exercise has three parts. First you confirm the failure that is left in the practice project. Second you write a test for a boundary, an input at the edge of what the method handles. Third you prove that the new test catches a bug.

## Part one: leave the failing test in place

1. Open Test Explorer, build with {{Ctrl+Shift+B}}, and click Run All.
2. Exactly one test fails: MinPrice_ReturnsTheSmallest. Do not fix it in this chapter. The code is wrong, and you fix it in Chapter 26.

## Part two: add a boundary test

Add this test to the class, after MinPrice_ReturnsTheSmallest:

```csharp
[Test]
public void Average_OfOneItem_IsThatPrice()
{
    decimal result = PriceCalculator.Average(new[] { 5m });
    Assert.That(result, Is.EqualTo(5m));
}
```

Before you run it, predict whether it will pass. Then build, and run it from Test Explorer. A list of one price is a boundary, the smallest list that is not empty.

## Part three: prove the test catches a bug

A passing test is not enough. Show that this test fails when the shortcut from the last lesson is in place.

1. In Average, change the return line to `return Total(prices) / 2m;`.
2. Build, and run all the tests. Note which ones fail. Average_OfOneItem_IsThatPrice should fail, and Average_OfTwoAndFour_IsThree should still pass.
3. Press {{Ctrl+Z}} to undo the change, and run all the tests again.

## Check your work

After part two, six tests run. Five pass, and MinPrice_ReturnsTheSmallest still fails. That failure is expected until Chapter 26.

~~~spoiler
The new test passes with the current code, because the current Average divides the total by `prices.Count`. With one price, the total is 5, and 5 divided by 1 is 5.

With the shortcut, the same test returns 2.5 instead of 5, so it fails. The test with two prices still passes, because 6 divided by 2 is 3. That is the lesson: one test with two prices cannot tell the correct method from the shortcut, but a test with one price can.

The failing MinPrice test is not a mistake in this exercise. It is the bug you find and fix in Chapter 26.
~~~
