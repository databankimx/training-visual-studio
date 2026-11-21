# Run the tests

Before you trust the red test, see it for yourself. Open Test Explorer with {{Ctrl+E}} then {{T}}, and choose Run All. The bar at the top counts the results. One test should show a red X.

Click the failing test, which is `MinPrice_ReturnsTheSmallest`, and read the message in the detail pane. The message says the test expected 1.5, but the method returned 9. That message is the most useful part of the window, because it names the input and the wrong answer.

Test Explorer shows the runner's own words, so use it as the evidence. Ask the question the message raises: is the test wrong, or is the code wrong? Work that out before you change either one. In Chapter 11 the test was the thing that was wrong. Here the test asks for the right answer, so the code is the suspect.

## Try it

1. Open Test Explorer with {{Ctrl+E}} then {{T}}, and choose Run All. Press {{Ctrl+R}} then {{A}} to run all tests.
2. Click `MinPrice_ReturnsTheSmallest`, and read the expected and actual values.
3. Write down the two values before you go on.
