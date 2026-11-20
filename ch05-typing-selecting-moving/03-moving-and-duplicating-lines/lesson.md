# Moving and duplicating lines

Code often needs to change order. A line sits above the line it should follow, or a statement belongs earlier in a method. You could cut and paste it, but moving the line directly is faster and leaves the clipboard alone.

## Moving a line with Alt+Up and Alt+Down

Put the cursor anywhere on the line. Press {{Alt+Up}} to move the line above the line before it, or {{Alt+Down}} to move it below the line after it. The cursor moves with the line, so you can press the key again and keep going. Here is a short example. The declaration of prices comes after the line that uses it, so the code will not compile. Put the cursor on the first line and press {{Alt+Down}}:

Before:

```csharp
decimal total = PriceCalculator.Total(prices);
var prices = new[] { 1m, 2m, 3m };
```

After:

```csharp
var prices = new[] { 1m, 2m, 3m };
decimal total = PriceCalculator.Total(prices);
```


You can also move several lines together. Select the lines first, then press {{Alt+Up}} or {{Alt+Down}}. The whole block moves as one.

Moving a line inside a method can break its structure. A line moved past a closing brace may end up outside the method. If the code stops looking right after a move, undo with {{Ctrl+Z}} and try again one line at a time.

## Duplicating a line with Ctrl+D

To copy a line, put the cursor on it and press {{Ctrl+D}}. Visual Studio inserts a copy directly below the original, and the cursor moves to the copy. You can then edit the copy without touching the original. Duplicating is useful for a repeated pattern, such as a second check that differs only in one value. Here is an example. The line below prints a total. Put the cursor on it and press {{Ctrl+D}}, then change the copy so it prints an average:

Before:

```csharp
Console.WriteLine("Total: " + total);
```

After pressing {{Ctrl+D}}:

```csharp
Console.WriteLine("Total: " + total);
Console.WriteLine("Total: " + total);
```

After changing the second line:

```csharp
Console.WriteLine("Total: " + total);
Console.WriteLine("Average: " + average);
```

## Try it

1. Open Pricing/PriceCalculator.cs and find the return line in the Total method.
2. Put the cursor on the return line and press {{Alt+Up}}. The return line moves above the line before it. Check that the method still reads correctly.
3. Press {{Ctrl+Z}} to put the line back.
4. Put the cursor on the line that declares total, and press {{Ctrl+D}}. A copy appears below it.
5. Press {{Ctrl+Z}} to remove the copy.
