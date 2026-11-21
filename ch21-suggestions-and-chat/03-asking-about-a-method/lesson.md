# Asking about a method

A good question names the code it is about. Select the method in the editor, then ask in the Chat window. The selected text goes with the question, so Copilot knows which method you mean.

Ask one clear question at a time. Questions such as What does this method return? or What happens when the list is empty? give answers you can check. A broad question, such as Is this code good?, gets a broad answer that is hard to check.

Read the answer against the code. Find each claim in the answer, and point to the line that supports it. If a claim has no matching line, the answer is wrong, even if it sounds right. Copilot can also describe what a method should do instead of what it does, so compare the answer with the actual return statements, and with the tests in Pricing.Tests.

## Try it

1. Select the whole Average method in PriceCalculator.cs.
2. Ask Copilot, What does this method return when the list is empty?
3. Find the line in the method that handles the empty list, and check the answer against it.
