# Homework: snippet and cleanup

This exercise writes a snippet for an NUnit test method, uses it in the practice solution, cleans the file, and then removes the test. It edits a test file, so it follows the same rules as any code change. Do not commit anything.

## Work through these steps in order

1. **Write the snippet.** Create testcase.snippet, using the XML from lesson 2 as a model. Change the Title to Test case, the Shortcut to testcase, and the Code section to the text below.
2. **Import it.** Open the Code Snippets Manager, set the Language to Visual C#, and import testcase.snippet.
3. **Insert it.** Open the test class in the Pricing.Tests project. Place the cursor inside the class, type testcase, and press {{Tab}} twice.
4. **Fill in the placeholders.** Name the test Sum_OfOneAndTwo_IsThree, use 1 + 2 as the actual value, and 3 as the expected value.
5. **Clean up the file.** Click the broom button on the status bar, choose Run Code Cleanup (Profile 1), and read the change in Git Changes.
6. **Run the test.** Open Test Explorer, and run the new test. It should pass.
7. **Remove the test.** Delete the test method you added, and check that Git Changes shows no change for that file.

The Code section of testcase.snippet is:

```csharp
[Test]
public void $name$()
{
    Assert.That($actual$, Is.EqualTo($expected$));
}
```

## Check your work

The test passes in Test Explorer, and when you remove it, Git Changes shows no change for the test file.

~~~spoiler
If the test does not appear, check that the snippet imported under Visual C# and that the test class is in the `Pricing.Tests` project. If the placeholders do not highlight, check that the names in the Literal section match the names in the code, with dollar signs around each one.

If Code Cleanup changed lines you did not expect, the profile on your computer may differ from the one your team uses. Undo the cleanup, and check the profile before you go on.

The test uses NUnit, so the file must already have the using `NUnit.Framework` line. Most test files in the practice solution have it.
~~~
