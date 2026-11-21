# Inline suggestions

An inline suggestion appears in grey text at the cursor, after you pause typing or ask for one. Figure 21.1 shows a suggestion for the body of a method, shown in grey after the cursor.

![Figure 21.1 - An inline suggestion in grey text at the cursor](images/ch21-inline-suggestion.png "width=100%")

*Figure 21.1 - An inline suggestion in grey text at the cursor*

Press {{Tab}} to accept the whole suggestion. It becomes ordinary text in the file, so you can edit it, undo it with {{Ctrl+Z}}, or commit it like anything else. Press {{Esc}} to reject it, and the grey text disappears without changing the file.

Copilot often offers more than one suggestion for the same spot. Cycle through them with the shortcut keys for next and previous suggestion, which Visual Studio shows in the suggestion's tooltip. Pick the one that matches what the code should do, not the one that looks longest.

Typing over a suggestion also works. If you keep typing, the grey text updates or disappears, so you do not have to reject it first.

## Try it

1. In PriceCalculator.cs, place the cursor on an empty line inside a method, and type a few characters of a line.
2. Wait for a suggestion, and read it before you accept it.
3. Press {{Esc}} to reject it, and check that the file has not changed.
