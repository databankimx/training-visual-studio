# Inserting a snippet

A snippet is a short piece of code with a name. Visual Studio inserts it at the cursor. Place the cursor on an empty line inside a class, and press {{Ctrl+K}} then {{Ctrl+X}}. The snippet picker opens, as Figure 24.1 shows, with folders of snippets on the left. Choose the Visual C# folder, then choose a snippet from the list, and press Enter to insert it.

![Figure 24.1 - The snippet picker](images/ch24-snippet-picker.png "width=50%")

*Figure 24.1 - The snippet picker*

Some snippets have placeholders. The names you need to fill in are highlighted. Type over the first highlight, press {{Tab}} to move to the next, and repeat until you are done. Each placeholder is a place where the snippet expects a name or a value.

To wrap code you have already selected, such as a block of statements, use {{Ctrl+K}} then {{Ctrl+S}} instead. That opens the surround picker, which offers snippets such as if and for blocks.

Inserting a snippet is a change to your file. If you change your mind, press {{Ctrl+Z}} to undo it.

## Try it

1. Open any C# file in the practice solution, and place the cursor on an empty line inside a class.
2. Press {{Ctrl+K}} then {{Ctrl+X}}, choose Visual C#, and pick the prop snippet if your list shows it.
3. Fill in the placeholders, and then press {{Ctrl+Z}} to undo the insert.
