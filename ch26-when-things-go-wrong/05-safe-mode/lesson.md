# Safe mode

Safe mode starts Visual Studio without extensions. It is a way to find out whether an extension is causing a problem. If the problem goes away in safe mode, an extension is the likely cause. If it stays, the problem is in Visual Studio itself or in your solution.

To start in safe mode, close Visual Studio, and start it from a PowerShell window with the /safemode switch:

```powershell
& "C:\Program Files\Microsoft Visual Studio\18\Community\Common7\IDE\devenv.exe" /safemode
```

Use the same devenv path as in the Activity Log lesson, with your edition's folder. Reproduce the problem. Then close Visual Studio, and start it normally.

If the problem was an extension, open Manage Extensions, as Chapter 22 showed, and disable the extension you suspect. Restart Visual Studio, and check whether the problem comes back.

## Try it

1. Read the /safemode command above, and find the devenv path for your edition.
2. Do not run it yet. Write down the steps you would use to reproduce a problem in safe mode.
