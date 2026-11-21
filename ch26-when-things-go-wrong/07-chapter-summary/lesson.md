# Chapter summary

Remember these when Visual Studio misbehaves:

- The Output window shows what the background tools did. The Git pane explains a failed push.
- The Activity Log records Visual Studio's own errors. Start with the /log switch to write it.
- Safe mode starts without extensions, so you can test whether one is the cause.

```quiz
Where do you look first for the reason a push failed?
○ The Error List
→ The Error List shows problems in your code and the editor, not Git commands.
◉ The Source Control - Git pane in the Output window
→ Yes. The Git commands and their results appear there.
○ The Window menu
→ The Window menu controls window layout, not messages.
```

```quiz
You suspect an extension is causing a problem. What should you do?
○ Uninstall Visual Studio and install it again.
→ That is far more than the test needs.
○ Reset the window layout.
→ A layout reset does not change extensions.
◉ Start Visual Studio in safe mode, and see if the problem goes away.
→ Yes. Safe mode runs without extensions, so you can test the suspect.
```

```quiz
What does the /log switch do when you start Visual Studio?
◉ It writes the Activity Log file, which records Visual Studio's own errors and warnings.
→ Yes. That file is the most detailed record of a problem.
○ It turns on the Output window.
→ The Output window is open from the View menu, not the switch.
○ It resets your settings.
→ Resetting settings is a different action, covered in Chapter 23.
```
