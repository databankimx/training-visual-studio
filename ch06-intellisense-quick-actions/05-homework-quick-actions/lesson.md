# Homework: fix two errors with Quick Actions

This exercise gives you a short class with two errors. Fix both with Quick Actions, not by typing the fixes yourself. The aim is to practice reading the menu and choosing the right fix.

## Set up the file

Create a new file in the Pricing project, named Homework.cs. Paste in this code, and save the file.

```csharp
namespace Pricing;

public static class Homework
{
    public static string Describe(IReadOnlyList<decimal> prices)
    {
        var builder = new StringBuilder();
        int rounded = PriceCalculator.Average(prices);
        builder.Append("Average: ").Append(rounded);
        return builder.ToString();
    }
}
```

The file has two errors. One is a name that has no using directive. The other assigns a decimal value to an int variable, which needs an explicit conversion.

## Work through these steps in order

1. **Build and read the errors.** Press {{Ctrl+Shift+B}} to build the solution. Open the Error List with Command Search, and read the two errors.
2. **Fix the missing using.** Put the cursor on StringBuilder, and press {{Ctrl+.}}. Choose the option that adds the using directive for System.Text.
3. **Fix the type mismatch.** Put the cursor on the line that declares rounded, and press {{Ctrl+.}}. Choose the option that converts the average to an int with an explicit cast.
4. **Check the result.** Read the line that declares rounded. The cast drops the decimal part of the average, so the output shows only the whole number.
5. **Build again.** Press {{Ctrl+Shift+B}}. The build should succeed with no errors.

## Check your work

Compare your file with the worked solution below. When you are done, delete Homework.cs from the Pricing project, so the practice solution is back to its original files.

~~~spoiler
Here is the worked solution, after both Quick Actions. The `Homework.cs` file should match it line for line.

```csharp
using System.Text;

namespace Pricing;

public static class Homework
{
    public static string Describe(IReadOnlyList<decimal> prices)
    {
        var builder = new StringBuilder();
        int rounded = (int)PriceCalculator.Average(prices);
        builder.Append("Average: ").Append(rounded);
        return builder.ToString();
    }
}
```

The using directive was added at the top of the file, and the cast was added to the line that declares rounded. For a list of 1, 2, and 4, the average is 2.33..., so Describe returns "Average: 2". The cast drops the decimal part rather than rounding, which is worth knowing when you choose a fix.
~~~
