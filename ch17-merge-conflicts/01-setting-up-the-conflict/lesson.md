# Setting up the conflict

To make a conflict, two branches must change the same line. Start by adding a small file on main. Create a file in the Pricing project named Labels.cs, and paste in this code:

```csharp
namespace Pricing;

public static class Labels
{
    public static string PriceLabel(decimal price)
    {
        return $"Price: {price:C}";
    }
}
```

Build with {{Ctrl+Shift+B}}, then stage the file in the Git Changes window and commit it on main with the message Add price label. Pushing is optional for this chapter.

Make sure the status bar shows main. The next lesson creates a branch from here, and changes the same line in two different ways.

## Try it

1. Create Labels.cs with the code above, and build the solution.
2. Stage the file, and commit it on main with the message Add price label.
3. Check the status bar, and confirm that the branch is main.
