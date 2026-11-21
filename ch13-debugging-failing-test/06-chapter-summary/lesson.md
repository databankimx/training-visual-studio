# Chapter summary

Remember these as you debug a failing test:

- Right-click a test in Test Explorer, and choose Debug Test(s) to run only that test under the debugger.
- A breakpoint condition makes the debugger pause only when an expression is true. The Breakpoints window lists every breakpoint, with its condition.
- Work out the expected answer by hand before you change anything. If your answer matches the test, the code is wrong. If it matches the code, the test is wrong.

```quiz
Which command starts one test under the debugger?
○ Run
→ Run executes the test without stopping at breakpoints.
◉ Debug Test(s)
→ Yes. Choose it from the right-click menu of the test in Test Explorer.
○ Clear Test Results
→ Clear Test Results removes the pass and fail marks. It does not start a test.
```

```quiz
You want a breakpoint to pause only when price is greater than 5. What do you add to it?
◉ A condition
→ Yes. The condition price greater than 5 makes the breakpoint pause only when it is true.
○ A second breakpoint on the same line
→ A second breakpoint on the same line would still pause for every price.
○ A hit count of 5
→ A hit count pauses on the nth time the line runs. It does not check the value of price.
```

```quiz
A test expects 17. Your hand calculation gives 18, and the code returns 18. What is wrong?
○ The code
→ The code returns 18, which matches your calculation.
○ The debugger
→ The debugger reports the values. It does not decide what the answer should be.
◉ The test
→ Yes. The expected value is the mistake, so correct the test.
```
