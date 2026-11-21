# Running tests in Test Explorer

Test Explorer lists every test in the solution, grouped by test project and class. It is the window where you run tests and see their results.

Open it from the Test menu, or press {{Ctrl+E}}, then {{T}}. The window usually docks beside the editor, like the other tool windows you met in Chapter 4.

Before you run anything, build the solution with {{Ctrl+Shift+B}}. The tests run the code as it was last built, so a build first makes sure the results match what you see in the editor.

Figure 11.2 shows the window after a run of all the tests. The bar at the top counts the results. A green check mark means a test passed. A red X means it failed.

![Figure 11.2 - Test Explorer after running all tests](images/ch11-test-explorer.png "width=75%")

*Figure 11.2 - Test Explorer after running all tests*

To run every test, click Run All at the top of the window, or press {{Ctrl+R}}, then {{A}}. The Run All button is the green play icon. To run one test, right-click its name and choose Run. Use a single test when you change one method and want a quick answer. The other tests keep the results they had before.

## Try it

1. Open Test Explorer with {{Ctrl+E}}, then {{T}}, and build the solution with {{Ctrl+Shift+B}}.
2. Click Run All. Four tests pass, and one fails: MinPrice_ReturnsTheSmallest. You will read its message in the next lesson.
3. Right-click Average_OfTwoAndFour_IsThree, and choose Run. Only that test runs. The others keep their last results.
