# Homework: add a boundary test

This exercise has three parts. First you fix the wrong expected value from the last lessons. Second you write a test for a boundary, an input at the edge of what the method handles. Third you prove that the new test catches a bug.

## Part one: fix the wrong test

1. Open PriceCalculatorTests.cs.
2. In Total_OfOneTwoThree_IsSeven, change 7m to 6m, and delete the comment above the test.
3. Build with {{Ctrl+Shift+B}}, and click Run All in Test Explorer. All five tests should pass.

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

All six tests pass, with the original Average method in place.

~~~spoiler
The new test passes with the current code, because the current Average divides the total by prices.Count. With one price, the total is 5, and 5 divided by 1 is 5.

With the shortcut, the same test returns 2.5 instead of 5, so it fails. The test with two prices still passes, because 6 divided by 2 is 3. That is the lesson: one test with two prices cannot tell the correct method from the shortcut, but a test with one price can.

Part one matters too. The test with 7m could never pass without a bug in the expected value, so it was always going to fail.
~~~
