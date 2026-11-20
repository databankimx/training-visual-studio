# Extracting a method

Extract Method moves a block of code into a new method, and replaces the block with a call to that method. Use it when the same steps appear more than once, or when a long method has a part that has a clear name of its own. The code does the same thing afterward, but it reads more clearly.

Figure 8.2 shows the Extract Method preview, with the new method and the call that replaces the selected code.

![Figure 8.2 - The Extract Method preview](images/ch08-extract-method-preview.png "width=75%")

*Figure 8.2 - The Extract Method preview*

## Extracting the code

1. Select the lines you want to move. They must form a complete piece of work, such as a loop and the statements inside it.
2. Press {{Ctrl+.}} with the selection active, and choose Extract method from the Quick Actions menu.
3. Read the preview. It shows the new method, and the call that will replace the selection.
4. Enter a name for the method, and apply the change.

## An example

Here is a loop from a method, before and after extraction. The loop adds up the prices. Extracting it gives the sum a name, and leaves the method body easy to read.

Before:

```csharp
decimal total = 0m;
foreach (decimal price in prices)
{
    total += price;
}
return total;
```

After, with the loop moved to a method named AddUp:

```csharp
decimal total = AddUp(prices);
return total;
```

The new method holds the loop, and returns the sum that the loop computed.

## Common mistake

Visual Studio works out the parameters and the return value from the selection. If the selected code uses a variable declared earlier in the method, that variable becomes a parameter. Check the preview to confirm that the parameters match what the new method needs.
