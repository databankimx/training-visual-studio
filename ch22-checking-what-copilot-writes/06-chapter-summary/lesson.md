# Chapter summary

Remember these when you check Copilot's work:

- You own the code you commit. Read it, run it, test it, and then decide.
- An explanation is a claim. Test it against values you know, and treat a mismatch as a sign that something is wrong.
- Write at least one test yourself. A test Copilot wrote can agree with its own suggestion.

```quiz
What is the first step of the review loop?
○ Commit it
→ Committing comes last, after the code has passed your checks.
◉ Read it
→ Yes. Ask what each line claims, and whether it fits the name and the comment.
○ Accept it with Tab
→ Accepting a suggestion is not a check. Read it first.
```

```quiz
Copilot wrote a test for a method, and the test passes. What does that show?
○ The code is correct.
→ A passing test shows the code agrees with that test, and nothing more.
○ The explanation is correct.
→ The explanation is a separate claim, and it still needs checking.
◉ Only that the code agrees with the test Copilot wrote.
→ Yes. Write at least one test yourself, using values you worked out by hand.
```

```quiz
A chat answer and the code disagree. What should you do?
◉ Run the code on values you know, and correct whichever side is wrong.
→ Yes. The running code and your tests decide which side is wrong.
○ Trust the chat answer, because it is fluent.
→ Fluent wording is not evidence that the claim is correct.
○ Ignore it, because the code compiles.
→ Compiling shows the syntax is valid, not that the behavior is right.
```
