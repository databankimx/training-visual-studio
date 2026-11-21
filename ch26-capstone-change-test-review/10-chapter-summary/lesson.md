# Chapter summary

Remember these about the capstone:

- Check the branch and the Git Changes list before you start. Leftover changes end up in commits without you choosing them.
- Read the expected and actual values in Test Explorer, and ask whether the test or the code is wrong. Use the debugger to find the line.
- Commit one clear change, and describe it in the pull request so a reviewer can check it.

```quiz
Before you change any code, what should you ask about a failing test?
○ Whether the test runs faster on another computer.
→ Speed is not the question. Look at the failure.
◉ Whether the test or the code is wrong, using the expected and actual values.
→ Yes. The message tells you what the test wanted and what the code gave.
○ Whether the fix can go straight to main.
→ Your team does not fix problems directly on main.
```

```quiz
You find that a test expects 1.5, and the code returns 9. What is the first thing to check?
○ Whether the test name is too long.
→ The name is not the problem here.
◉ Which line in the code produces 9, using the debugger.
→ Yes. The debugger shows the line and the values that lead to the wrong answer.
○ Whether to delete the test.
→ The test asks for the right answer. Do not delete it to hide the failure.
```

```quiz
What should a pull request description contain?
○ Only the title, because the diff explains everything.
→ A reviewer should not need to reconstruct the reason from the code.
○ The number of lines you typed.
→ Line counts do not explain the change.
◉ What was wrong, what changed, and how you checked it.
→ Yes. A reviewer can check the fix from those three things.
```
