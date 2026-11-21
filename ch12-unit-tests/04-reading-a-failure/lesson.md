# Reading a failure

When a test fails, the most useful information is in its message. Click MinPrice_ReturnsTheSmallest in Test Explorer. The detail pane on the right shows the message, which says the expected value was 1.5, but the method returned 9.

Figure 12.3 shows the message in the detail pane.

![Figure 12.3 - The failure message in the Test Explorer detail pane](images/ch12-failure-message.png "width=85%")

*Figure 12.3 - The failure message in the Test Explorer detail pane*

Read the message in two halves. Expected is the value the test asked for. Was is the value the method returned. The message tells you that the two differ, but it does not tell you which side is wrong. You decide that by reading the code and the test.

Double-click the test name. Visual Studio opens PriceCalculatorTests.cs at the line of the failing assertion. Read the test. It passes the prices 1.5, 9, and 3 to MinPrice, and the smallest of those is 1.5. The test is right. The method returned 9, which is the largest price, so the code is wrong.

A common mistake is to change the test so it passes, by changing the expected value to 9. The test would pass, and the program would be wrong. A test is a claim about what the code should do. When the claim is wrong, fix the test. When the code is wrong, fix the code. The message is where you start, not where you stop.

## Try it

1. Click the failing test in Test Explorer, and read the message in the detail pane.
2. Double-click the test name to open the file at the failing line.
3. Read the test. Do not change anything yet. You will find the cause and fix the code in Chapter 26.
