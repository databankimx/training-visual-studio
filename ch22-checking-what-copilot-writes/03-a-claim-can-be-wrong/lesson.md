# A claim can be wrong

Copilot also explains code, and an explanation is a claim you can check. Figure 22.1 shows a chat exchange about a method that totals the prices in a list. Copilot's answer says the method adds each price to a running total. The sum it mentions is correct, but the method does not do what the answer says.

![Figure 22.1 - A chat answer that says the method adds every price, marked where the code disagrees](images/ch22-wrong-claim.png "width=75%")

*Figure 22.1 - A chat answer that says the method adds every price, marked where the code disagrees*

Here is the method, in a file of its own:

```csharp
public static decimal Total(IReadOnlyList<decimal> prices)
{
    decimal total = 0m;
    foreach (decimal price in prices)
    {
        total = price;
    }
    return total;
}
```

The loop itself is fine, and the answer sounds right. Do not stop there. Run the method on the same four prices, 12.50, 8.00, 3.75, and 20.00. The sum is 44.25. The method returns 20.00, because the line inside the loop replaces the total on every pass, instead of adding to it. The fix is `total += price;`.

The claim was wrong, and the code was the thing to trust. Test the claim against values you know, and when the two disagree, change the claim in your notes, not the expected answer.

## Try it

Read the method above. Without running it, write down the value it returns for the list 2, 4, and 6. Then check your answer by running it.
