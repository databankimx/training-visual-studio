# Import and export settings

Your settings are stored on your computer. Visual Studio can save them to a file, so you can move them to another computer, or keep a copy before you change a lot. Open the Tools menu, and choose Import and Export Settings. A wizard opens and asks what you want to do.

To export, choose Export selected environment settings, and then choose the groups to include. You can take everything, or only the groups you want. The wizard asks where to save the file. Settings files use the .vssettings extension. Save it somewhere you will find again, such as your Documents folder, and not inside a repository.

To import, choose Import selected environment settings, and browse to a .vssettings file. Before the import, the wizard offers to save your current settings first. Take that offer. Once a file is imported, its settings replace the matching ones on your computer.

Reset all settings is a third option. It returns Visual Studio to its defaults. Use it only when you are sure you want to lose your current choices.

A settings file is a text file in XML format, and it records your choices. It can also record folder paths and account names from your computer. Open it and read it before you send it to anyone. Never put it in a repository that other people can see.

## Try it

1. Open the Tools menu, and choose Import and Export Settings. Choose Export selected environment settings, and save the file to your Documents folder as my-settings.vssettings.
2. Open that file in Notepad, and scroll through it. Close Notepad without changing anything.
3. Open the wizard again, and choose Cancel when it asks what to import.
