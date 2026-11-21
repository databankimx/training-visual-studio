# Chapter summary

Remember these as you work with tests:

- A test is a method with the [Test] attribute. It calls the code with known input, and checks the result with Assert.That.
- The Test menu lists every test command with its shortcut. {{Ctrl+R}}, then {{A}}, runs all the tests, and {{Ctrl+E}}, then {{T}}, opens Test Explorer.
- Test Explorer shows the results. A green check mark means a pass, and a red X means a failure.
- The failure message shows the expected value and the value the method returned. Decide whether the code or the test is wrong.
- A passing test proves only the inputs it uses. Choose inputs that differ, and include the edge cases.

```quiz
Which attribute marks a method as one test in NUnit?
○ [TestFixture]
→ [TestFixture] marks the class that groups the tests. It does not mark one test.
○ [SetUp]
→ [SetUp] runs before each test, but it is not a test itself.
◉ [Test]
→ Yes. Each method with [Test] above it runs as one test in Test Explorer.
```

```quiz
A test fails. Where do you look first to see the expected value and the value the method returned?
◉ The failure message in the Test Explorer detail pane
→ Yes. The message shows Expected and Was for the failing assertion.
○ The Output window
→ The Output window shows build and debug messages. It does not show test results.
○ The Breakpoints window
→ The Breakpoints window lists breakpoints, not test results.
```

```quiz
A test passes. Which statement is true?
○ The method is correct for every possible input.
→ A passing test only proves the inputs in that test.
○ The test cannot fail later.
→ A test can fail later, when the code changes in a way it does not expect.
◉ The method returned the expected value for the inputs in that test.
→ Yes. Other inputs may still expose a bug, so add tests for the edge cases.
```
