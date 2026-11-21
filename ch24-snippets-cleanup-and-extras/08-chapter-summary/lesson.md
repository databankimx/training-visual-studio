# Chapter summary

Remember these about snippets, cleanup, and Quick Launch:

- Ctrl+K then Ctrl+X inserts a snippet, and Ctrl+K then Ctrl+S surrounds selected code with one.
- A snippet is an XML file with a shortcut, placeholders, and code. Import it with the Code Snippets Manager.
- Code Cleanup changes the text of a file, so read the change in Git Changes before you commit.
- Quick Launch, opened with Ctrl+Q, finds commands and settings. Some results open the older separate window.

```quiz
Which shortcut inserts a snippet at the cursor?
○ Ctrl+K then Ctrl+S
→ That shortcut surrounds selected code with a snippet.
○ Ctrl+Q
→ Ctrl+Q opens Quick Launch, the search box.
◉ Ctrl+K then Ctrl+X
→ Yes. Ctrl+K then Ctrl+X opens the snippet picker, and Ctrl+K then Ctrl+S is the surround version.
```

```quiz
You turn on cleanup on save, and a saved file shows a change you did not make. What should you do?
◉ Undo the change, check the profile, and read the diff before you commit.
→ Yes. Cleanup changes the text, so check what it did before you continue.
○ Commit it anyway, because cleanup is always right.
→ Cleanup applies the rules it is given, which may not match your intent.
○ Turn off Git, because it shows changes you did not make.
→ Git is showing you the change. Read it.
```

```quiz
You want a snippet that inserts a test method. Where is the code kept, and how do you make it available?
○ In the Solution Explorer, and it is available at once.
→ The Solution Explorer shows files, not snippets.
○ In a Git branch, and you switch to it.
→ Branches hold your code changes, not the snippet picker.
◉ In a .snippet file, imported with the Code Snippets Manager.
→ Yes. Import the file, and the snippet appears in the picker.
```
