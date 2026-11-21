# Chapter summary

The checklist covers the whole course. The habits behind it are simple: know what state you are in, check what you change, test before you trust, and review before you share.

- Start from a clean state, and know which branch you are on.
- Test before you trust a result, whether it came from you, from a tool, or from Copilot.
- Commit only what you checked, and write the message for the reader who comes after you.
- Publish and open a pull request so a second person can see the change.
- When something goes wrong, read the Output window and the Error List first, then the Activity Log, then safe mode.

The appendix at the end lists the shortcuts and commands the lessons used.

```quiz
Why does the checklist start with checking the branch and the Git Changes window?
○ Because Visual Studio cannot open a solution without it.
→ Visual Studio opens solutions either way. The check is about your work.
◉ Because leftover changes would end up in your commit without you choosing them.
→ A clean start means every change you commit is one you decided on.
○ Because the branch name is used by the tests.
→ The tests do not depend on the branch name.
```

```quiz
A test fails after an edit. What is the right order of steps?
◉ Read the expected and actual values, debug with a breakpoint, then fix the cause.
→ Work out which side is wrong, then change that side, and run the tests again.
○ Whether the test runs faster after a restart.
→ Speed is not the question.
○ Delete the test, so the run passes.
→ Deleting a test hides the problem. Read the expected and actual values instead.
```

```quiz
Visual Studio shows an error you cannot explain. Where do you look first?
○ The Options dialog.
→ Options holds settings, not error messages.
○ The shortcut list.
→ Shortcuts do not record errors.
◉ The Output window and the Error List.
→ Yes. They show messages from the tools and from your code, and they are the quickest place to look.
```
