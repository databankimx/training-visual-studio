# Homework: resolve the conflict

This exercise has you resolve the conflict from the last lesson, and explain why.

## Work through these steps in order

1. **Decide the wording.** Which should the label say: Listed price with two decimal places, or Cost with the default currency format? Write your answer in one sentence before you change the file.
2. **Try an option.** In the merge editor, tick the Current checkbox, then the Incoming checkbox, then both, and watch the Result pane. Untick the boxes before you try the next option.
3. **Choose one result.** Tick the version you want, or edit the line in the Result pane so that it has one return statement.
4. **Build.** Build with {{Ctrl+Shift+B}}. The file should build with no markers and no warnings.
5. **Accept and commit.** Click Accept Merge, stage Labels.cs, and write a commit message that explains the choice, such as Keep listed price wording for labels. Commit the merge.

## Explain each choice

Write one sentence for each option you tried, saying why you kept it or why you did not. Put the sentences in the commit message body, below the first line.

## Check your work

Labels.cs contains a single return line, the history shows the merge commit, and the Git Changes window has no conflicts.

~~~spoiler
Ticking the Current checkbox keeps Listed price with two decimal places, and the file builds cleanly.

Ticking the Incoming checkbox keeps Cost with the default format. It builds, but it drops the two decimal places you asked for on main.

Ticking both checkboxes puts two return statements in a row. The first one always runs, so the second is unreachable, and the compiler warns about it. Keeping both looks safe, but it leaves code that is never used.

Either a current or an incoming choice is a correct resolution. What matters is the decision you record in the commit message.

Keep Labels.cs. Chapter 18 uses its history, so do not delete it.
~~~
