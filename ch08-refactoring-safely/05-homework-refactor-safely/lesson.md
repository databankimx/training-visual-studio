# Homework: rename, extract, and tidy

This exercise gives you a short class in which one method is called three times. You rename the method so its name says what it does, then pull the repeated call into a local variable. The class does the same thing at each step, so you can check your work by building it.

## Set up the file

Create a new file in the Pricing project, named Refactor.cs. Paste in this code, and save the file.

```csharp
namespace Pricing;

public static class Refactor
{
    public static decimal Describe(IReadOnlyList<decimal> prices)
    {
        decimal a = Calc(prices) * 2m;
        decimal b = Calc(prices) + 1m;
        decimal c = Calc(prices) - 1m;
        return a + b + c;
    }

    public static decimal Calc(IReadOnlyList<decimal> prices) => prices.Sum();
}
```

## Work through these steps in order

1. **Rename the method.** Put the cursor on Calc in its declaration, and press {{Ctrl+R}}, then {{Ctrl+R}}. Type SumOfPrices, and turn on the preview. Check that all three calls in Describe are listed, and press {{Enter}}.
2. **Pull the repeated call into a variable.** Select the call SumOfPrices(prices) in the first line of Describe. Press {{Ctrl+.}}, and choose the option that introduces a local variable.
3. **Use the variable.** Replace the other two calls to SumOfPrices(prices) with the variable name.
4. **Check the result.** Read Describe. It should call SumOfPrices once, and use the variable in the three calculations.

## Check your work

Press {{Ctrl+Shift+B}} to build the solution. The build should succeed. Compare your file with the worked solution below.

When you are done, delete Refactor.cs from the Pricing project, so the practice solution is back to its original files.

~~~spoiler
Here is the worked solution, after all four steps. The `Refactor.cs` file should match it line for line, although the name of the local variable may differ if you chose a different one.

```csharp
namespace Pricing;

public static class Refactor
{
    public static decimal Describe(IReadOnlyList<decimal> prices)
    {
        decimal sum = SumOfPrices(prices);
        decimal a = sum * 2m;
        decimal b = sum + 1m;
        decimal c = sum - 1m;
        return a + b + c;
    }

    public static decimal SumOfPrices(IReadOnlyList<decimal> prices) => prices.Sum();
}
```

The rename changed the declaration and all three calls in one step, which is why the preview is worth reading first. The local variable means the sum is worked out once, and the three calculations use its value.
~~~
