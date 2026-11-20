# 12. Debugging a Failing Test

Chapter 11 showed how to read a failure. The next step is to find out why the code gives the wrong answer. A failing test is a good place to start, because the test already names the input and the answer it expects. You set a breakpoint in the code the test calls, start the test under the debugger, and watch the values until the wrong one appears.

Finding the wrong value is only half the job. You still have to decide which side is wrong, the code or the test. This chapter covers starting one test under the debugger, the Breakpoints window, and how to make that decision. The exercises add a small discount method to the practice solution, with two tests for it.
