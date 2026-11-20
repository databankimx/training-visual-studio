# Chapter summary

These tools change the structure of code while keeping its behavior:

- Rename a symbol with {{Ctrl+R}}, then {{Ctrl+R}}. Every use changes with it.
- Open the drop-down in the Rename box to preview the changes before you apply them.
- Extract Method moves a selected block to a new method, through the Quick Actions menu with {{Ctrl+.}}.
- Code Cleanup, with {{Ctrl+K}}, then {{Ctrl+E}}, applies style and analyzer fixes to a file.

```quiz
Which key combination starts a rename of the symbol under the cursor?
○ Ctrl+F
→ Ctrl+F opens the Find box for the current file. Rename is Ctrl+R, then Ctrl+R.
◉ Ctrl+R, then Ctrl+R
→ Yes. Type the new name in the Rename box, and press Enter to apply it.
○ Ctrl+H
→ Ctrl+H opens Replace. Replace changes text, but it does not update each use of a symbol.
```

```quiz
What does the preview in the Rename box show you?
○ The new name, before you type it
→ The preview comes after you type the new name, and it lists the changes.
◉ A list of the changes, grouped by file, before the rename is applied
→ Yes. Read the list, and then press Enter to apply the rename, or Cancel to stop.
○ The output of a build
→ Build output appears in the Output window. The preview lists the changes to the code.
```

```quiz
What does Extract Method do with a selected block of code?
○ It deletes the block
→ Extract Method keeps the code. It moves it to a new method, and calls that method in its place.
◉ It moves the block into a new method, and replaces it with a call
→ Yes. The code does the same thing afterward, but the new method has its own name.
○ It formats the whole file
→ Formatting changes layout only. Extract Method moves the selected block into a new method.
```
