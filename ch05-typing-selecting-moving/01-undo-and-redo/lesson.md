# Undo and redo

Mistakes happen while you type, and most of the time the fastest fix is to undo. Undo reverses your last change, one step at a time. Redo puts back a change you have just undone. Between them, you can move back and forth through your recent edits without retyping anything.

## Undo with Ctrl+Z

Press {{Ctrl+Z}} to undo. Each press steps back through your recent changes in the open file. Visual Studio groups some keystrokes together, so one press may remove a whole word rather than a single letter. The grouping is decided by Visual Studio, so watch the screen after each press to see what it removed.

## Redo with Ctrl+Y

Press {{Ctrl+Y}} to redo. It brings back the change you last undid. Redo only works until you type something new. Once you type after an undo, the changes you undid are gone from the redo history.

## Try it

1. Open Pricing/PriceCalculator.cs. It is the file that holds the Total method.
2. Click at the end of the line that reads decimal total = 0m;.
3. Type a space, then // test. Notice that the text is added at the cursor.
4. Press {{Ctrl+Z}} once. The text you typed should disappear. If it does not disappear all at once, press {{Ctrl+Z}} again until the line is back to what it was.
5. Press {{Ctrl+Y}} once. The text returns.
6. Press {{Ctrl+Z}} again to remove it, so the file is back to its original state.

## Undo from the Edit menu

Undo and Redo are also on the Edit menu, near the top of the window. Use the menu when you want to see the command name, or when you have forgotten the key. The menu item shows the shortcut beside it, so the menu is also a quick way to learn the keys.

## Common mistake

People often press {{Ctrl+Z}} too many times and go back past the change they meant to keep. If that happens, press {{Ctrl+Y}} until the change is back. Stop before you type anything new, because typing clears the redo history.

Undo covers the open file only. It does not reverse changes you made in other files, so keep that in mind when you work across the solution.
