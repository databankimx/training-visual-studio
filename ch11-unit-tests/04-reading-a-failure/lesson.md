# Reading a failure

When a test fails, the most useful information is in its message. Click Total_OfOneTwoThree_IsSeven in Test Explorer. The lower pane shows the message, which says the expected value was 7, but the method returned 6.

Figure 11.3 shows the message in the detail pane.

![Figure 11.3 - The failure message in the Test Explorer detail pane](images/ch11-failure-message.png "width=75%")

*Figure 11.3 - The failure message in the Test Explorer detail pane*

Read the message in two halves. Expected is the value the test asked for. Was is the value the method returned. The message tells you that the two differ, but it does not tell you which side is wrong. You decide that by reading the code and the test.

Double-click the test name. Visual Studio opens PriceCalculatorTests.cs at the line of the failing assertion. Read the comment above the test: the expected value is deliberately wrong. The prices are 1, 2, and 3, and their total is 6. The code is right, and the test is wrong.

A common mistake is to change the code so the test passes. If you made Total return 7 for those three prices, the test would pass, and the program would be wrong. A test is a claim about what the code should do. When the claim is wrong, fix the test. When the code is wrong, fix the code. The message is where you start, not where you stop.

## Try it

1. Click the failing test in Test Explorer, and read the message in the detail pane.
2. Double-click the test name to open the file at the failing line.
3. Read the comment above the test. Do not change anything yet. You will fix this test in the homework.
