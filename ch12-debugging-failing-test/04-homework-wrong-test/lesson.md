# Homework: find the wrong test

This exercise has a test that is wrong, and code that is right. Your job is to prove it with the debugger, and fix the test.

## Add the test

Add this test to DiscountsTests.cs, after the zero-percent test:

```csharp
[Test]
public void ApplyPercent_FifteenPercentOffForty_IsThirtyThree()
{
    decimal result = Discounts.ApplyPercent(40m, 15m);
    Assert.That(result, Is.EqualTo(33m));
}
```

## Work through these steps in order

1. **Work out the answer.** Fifteen percent of 40 is how much? Subtract it from 40. Write down the result before you run anything.
2. **Run the test.** Build, and run it from Test Explorer. Read the failure message. Does the expected value match your answer?
3. **Debug the code.** Set a breakpoint on the return line in Discounts.cs. Debug the test from its right-click menu. Read the values in the Locals window, and check that the code returns your answer.
4. **Decide.** The code is right, so the test is wrong. Say so in one sentence before you change anything.
5. **Fix the test.** Change the expected value to the correct answer, and run all the tests.

## Check your work

All the tests in DiscountsTests.cs should pass, and the Locals window should match your hand calculation at the return line.

~~~spoiler
Fifteen percent of 40 is 6, and 40 minus 6 is 34. The test expected 33, so the test is wrong, and the code is right.

At the return line, the Locals window shows price as 40, and discount as 6. The method returns 34. Change the test to expect `34m`, and run all the tests.

When you finish, delete `Discounts.cs` and `DiscountsTests.cs`, unless your instructor asks you to keep them.
~~~
