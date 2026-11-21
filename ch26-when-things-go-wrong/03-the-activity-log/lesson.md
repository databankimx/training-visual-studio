# The Activity Log

The Activity Log is a file that Visual Studio writes as it runs. It records errors, warnings, and information from its own components, with the time and the component that wrote each entry. It is the most detailed record of a problem, and it is the first thing to give a support team when you report one.

To write the log, close Visual Studio, and start it from a PowerShell window with the /log switch. The /log switch needs a file name after it, which is the full path where Visual Studio should save the log. Put the switch at the end of the command. The path to devenv depends on your edition, and the command looks like this:

```powershell
& "C:\Program Files\Microsoft Visual Studio\18\Community\Common7\IDE\devenv.exe" /log "C:\Temp\ActivityLog.xml"
```

The folder in the path must exist before you start Visual Studio. If it does not, create it first with `New-Item -ItemType Directory -Force -Path C:\Temp`.

Do not use your Documents folder for this. On many computers Documents is redirected to OneDrive, so the path may not point where you expect, and the log can fail to write there.

Visual Studio writes the log while it runs. Naming the path yourself tells you exactly where the file is. The example writes ActivityLog.xml to C:\Temp, and you can choose a different name. Figure 26.1 shows part of it. Each entry has a type, such as Error, Warning, or Information, and a description. Search the file for the word Error to find the first problem.

![Figure 26.1 - Part of the Activity Log file](images/ch26-activity-log.png "width=75%")

*Figure 26.1 - Part of the Activity Log file*

The log can contain folder paths and account names from your computer. Read it before you send it to anyone.

## Try it

1. Close Visual Studio, and start it with the /log switch and the path in C:\Temp, from PowerShell.
2. Open C:\Temp\ActivityLog.xml in Notepad.
3. Search for Error, and read the first entry you find. Close the file without changing it.
