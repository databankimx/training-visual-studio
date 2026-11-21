# Homework: fix a build in order

This exercise gives you a short class with two errors. Build it, read the Error List, and fix the errors in the order they appear in the file. The first fix should remove more than one error from the list.

## Set up the file

Create a new file in the Pricing project, named BuildPractice.cs. Paste in this code, and save the file.

```csharp
namespace Pricing;

public static class BuildPractice
{
    public static int Double(int value)
    {
        return value * 2
    }

    public static string Greeting()
    {
        return Helo;
    }
}
```

## Work through these steps in order

1. **Build and open the Error List.** Press {{Ctrl+Shift+B}}, then open the Error List with Command Search. Read the errors, and note the line of each one.
2. **Fix the first error.** The return line in Double is missing a semicolon at its end. Add the semicolon, and build again.
3. **Fix the second error.** The name Helo is not a string in quotation marks, so the compiler cannot find it. Change the line to return the text Hello, in quotation marks.
4. **Build in Release.** Change the configuration dropdown to Release, and press {{Ctrl+Shift+B}}. Check that the Output window shows the Release folder.
5. **Change back to Debug.** Set the dropdown back to Debug.

## Check your work

The build should succeed with no errors. Compare your file with the worked solution below.

When you are done, delete BuildPractice.cs from the Pricing project, so the practice solution is back to its original files.

~~~spoiler
Here is the worked solution, after both fixes. The `BuildPractice.cs` file should match it line for line.

```csharp
namespace Pricing;

public static class BuildPractice
{
    public static int Double(int value)
    {
        return value * 2;
    }

    public static string Greeting()
    {
        return "Hello";
    }
}
```

The missing semicolon was the first error in the file, and fixing it first was the right order. The name Helo was a separate mistake, and it needed a text value in quotation marks. Each fix was small, and the build reported both in the Error List.
~~~
