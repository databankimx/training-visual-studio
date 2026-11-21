# Homework: explain the change

Write the description for your pull request. A good description lets a reviewer understand the change without asking you a question, and it tells them how you know the change works.

## Work through these steps in order

1. **Write a title.** Use the same wording as your commit message.
2. **Say what was wrong.** Name the method, and the wrong answer it gave for the test's input.
3. **Say what you changed.** Name the line, and why the new version is correct.
4. **Say how you checked.** Name the tests you ran, and say they all pass.
5. **Open the pull request**, and paste the description.

## Check your work

The description names `MinPrice`, the input that failed, the change, and the test run. A reviewer who has not seen your screen could check the fix from it.

~~~spoiler
A short example: "`MinPrice` returned the largest price, because it called `Max`. Changed it to `Min`. `MinPrice_ReturnsTheSmallest` expects 1.5 for the prices 1.5, 9, and 3, and every test in the solution passes."

A description that says "fixed the bug" is not enough. The reviewer has to read the diff to find out which bug, and which fix.
~~~
