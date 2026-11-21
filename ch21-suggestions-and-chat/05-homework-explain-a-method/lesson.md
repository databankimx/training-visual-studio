# Homework: explain a method

This exercise has you ask Copilot to explain a method, and then check each claim in the answer. The code is practice code, so it is safe to paste into the chat.

## Work through these steps in order

1. **Select the method.** In PriceCalculator.cs, select the whole Total method.
2. **Ask.** In the Chat window, ask, What does this method return, and what happens when the list is empty?
3. **Read the answer.** Write down each claim it makes, one per line.
4. **Check each claim.** For each claim, find the line in the method that supports it. Mark it as correct, wrong, or not in the code.
5. **Check the tests.** Open Pricing.Tests, and find the test for the empty list. Check that its expected value matches the answer.

## Check your work

Every claim in the answer is marked, and you can point to the line or test behind each correct one.

~~~spoiler
Total adds each price to a running total, which starts at zero, and returns the total. For an empty list, the loop never runs, so the method returns zero. The test Total_OfEmptyList_IsZero checks that value.

If the answer said something the code does not do, such as sorting the prices or rounding the result, the claim is wrong, and you should say so in your notes.

A correct answer does not prove the code is right. It only shows that the explanation matches what the code does, which is still worth checking against the tests.
~~~
