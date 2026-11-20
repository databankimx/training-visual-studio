# Code or test?

The debugger tells you what the code did. It cannot tell you what the code should have done. For that, you need a value you know is right, and you get it by working the answer out by hand.

Take the failing test from the first lesson. It expects 18 when 10 percent is taken from 20. Ten percent of 20 is 2, and 20 minus 2 is 18, so the test is right. The code is wrong. The debugger showed discount as 200, but the discount should be 2. The code multiplies the price by the percent, and it never divides by 100. The fix is one change:

```csharp
decimal discount = price * percent / 100m;
```

Now take a different case. Suppose a test expects 17 for 20 with 10 percent off. Your hand calculation gives 18, and the code returns 18. The code is right, and the test has a wrong expected value. A test can be wrong for the same reasons code can be wrong: a typo, a copied number, or a misreading of the rule.

Use this order each time a test fails:

1. Before you look at the code, work out the expected answer by hand, with the same inputs.
2. If your answer matches the test, the code is wrong. Use the debugger to find the line.
3. If your answer matches the code, the test is wrong. Fix the expected value, and say why in the test name or a comment.

Changing the code to match a wrong test is the mistake to avoid. The test is a claim, and you check it before you act on it.

## Try it

1. Make the fix in Discounts.cs shown above, and build with {{Ctrl+Shift+B}}.
2. Run all the tests with {{Ctrl+R}}, then {{A}}. Both tests should now pass.
