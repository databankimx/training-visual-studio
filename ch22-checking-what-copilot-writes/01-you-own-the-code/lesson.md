# You own the code

When you commit code, you are saying that you have read it, understand it, and can explain and support it. That statement does not change because a tool wrote part of it. If a suggestion breaks the build, or a test fails in production, the answer "Copilot wrote it" does not help anyone fix it.

The development rules for custom code at DataBank say the same thing. Every developer must understand the code they deliver, and AI-assisted code gets the same review as hand-written code. A reviewer should not approve code just because it compiles or looks tidy. Polished output is not evidence of correctness.

This is why a review has to check behavior, not appearance. A suggestion can be formatted well, use good names, and still return the wrong answer for an empty list. Your job is to find that answer before the code leaves your computer.

Before you keep a suggestion, ask yourself whether you could explain every line to a reviewer, and whether you know what it returns for an empty input, a single item, and a typical case. If you cannot answer, the suggestion is not ready.
