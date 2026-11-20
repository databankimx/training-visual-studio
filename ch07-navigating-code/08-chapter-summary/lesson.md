# Chapter summary

These keys cover most of the navigation you will do in this course:

- Go to Definition, with {{F12}}, takes you from a call to its declaration. Navigate Back, with {{Ctrl+-}}, takes you back.
- Find All References, with {{Shift+F12}}, lists every use of a name in the solution.
- Peek Definition, with {{Alt+F12}}, shows a definition inside the file you are working in.
- CodeLens shows a reference count above each declaration, and clicking it opens the list.
- The Object Browser, from the View menu, lists the types and members of libraries.

```quiz
Which key moves the cursor from a method call to its declaration?
○ Shift+F12
→ Shift+F12 lists every use of the name. It does not move you to the declaration.
○ Alt+F12
→ Alt+F12 shows the declaration in a box, in the same file. F12 opens the file itself.
◉ F12
→ Yes. Go to Definition opens the file that declares the method, with the cursor on it.
```

```quiz
What does Find All References show?
◉ Every place the name is used in the solution
→ Yes. Each result shows the file and the line, and you can open any of them.
○ Only the declaration of a name
→ Find All References lists the uses of the name, so the list is longer than the declaration alone.
○ The version history of a file
→ Version history comes from Git, which the course covers later. Find All References lists the uses of a name.
```

```quiz
Which keys bring you back to where you were before a Go to Definition?
○ Ctrl+Z and Ctrl+Y
→ Ctrl+Z and Ctrl+Y undo and redo text changes. They do not move the cursor.
◉ Ctrl+- and Ctrl+Shift+-
→ Yes. Ctrl+- goes back through the places you visited, and Ctrl+Shift+- goes forward again.
○ Ctrl+Q and Ctrl+T
→ Ctrl+Q opens Command Search, and Ctrl+T opens Go to All. Neither goes back.
```
