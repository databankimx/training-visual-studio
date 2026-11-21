# Homework: tidy a class

This exercise gives you a messy class to clean up with the keys from this chapter. The code is valid, so it builds. It is untidy on purpose, so you can practice the editing keys on real code.

## Set up the starter file

Create a new file in the Pricing project, named Starter.cs. Paste in this code, and save the file.

```csharp
using System;
namespace Pricing {
public class Starter {
public static decimal Discounted(decimal price,decimal rate){
if(rate<0m||rate>1m){throw new ArgumentOutOfRangeException("rate");}
decimal discount=price*rate;
return price-discount;
}
public static decimal Tax(decimal price){
decimal tax=price*0.08m;
return price+tax;
}
}
}
```

Read the code once before you change it. The braces do not line up, each statement is crammed onto a line with the others, and the Tax method sits below the Discounted method, which is the order you will change.

## Work through these steps in order

1. **Format the file.** Press {{Ctrl+K}}, then {{Ctrl+D}}. Check that the braces and indentation now line up, and that each statement sits on its own line.
2. **Move the Tax method above the Discounted method.** Select the five lines of the Tax method, from its signature to its closing brace. Press {{Alt+Up}} once for each line the method has to pass. Stop when the Tax method sits above the Discounted method. Use {{Ctrl+Z}} if you go too far.
3. **Duplicate a line, then undo the copy.** Put the cursor on the line that reads decimal discount=price*rate;, and press {{Ctrl+D}}. A copy appears below it. Press {{Ctrl+Z}} to remove the copy, so the method is back to one discount line.
4. **Comment out the tax line.** Select the line that reads decimal tax=price*0.08m;, and press {{Ctrl+K}}, then {{Ctrl+C}}.
5. **Uncomment it.** Select the same line, and press {{Ctrl+K}}, then {{Ctrl+U}}.

## Check your work

Press {{Ctrl+Shift+B}} to build the solution. The build should succeed with no warnings. Then compare your file with the worked solution below, line by line.

When you are done, delete Starter.cs from the Pricing project, so the practice solution is back to its original files.

~~~spoiler
Here is the worked solution, after all five steps. The `Starter.cs` file should match it line for line.

```csharp
using System;
namespace Pricing
{
    public class Starter
    {
        public static decimal Tax(decimal price)
        {
            decimal tax = price * 0.08m;
            return price + tax;
        }
        public static decimal Discounted(decimal price, decimal rate)
        {
            if (rate < 0m || rate > 1m)
            {
                throw new ArgumentOutOfRangeException("rate");
            }
            decimal discount = price * rate;
            return price - discount;
        }
    }
}
```

Step 1 changed only the layout. Step 2 moved the Tax method, which is why it now comes first. Steps 3 to 5 left the code as it was, because the duplicate was removed with undo and the comment was removed again.
~~~
