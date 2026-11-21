# Homework: remove the package, then add it back at a new version

This exercise removes Newtonsoft.Json from `Pricing`, then adds it back at 13.0.4, and checks the project file each time. Work in your practice solution. The package should be at 13.0.3 before you start, from the last lesson.

1. Confirm the starting point. Open `Pricing.csproj`, and check that its `PackageReference` shows `Version="13.0.3"`.
2. Remove the package. Right-click `Pricing`, choose **Manage NuGet Packages**, and go to the **Installed** tab. Choose Newtonsoft.Json, and remove it.
3. Check the removal. Open `Pricing.csproj`. The `PackageReference` line for Newtonsoft.Json should be gone.
4. Add it back at 13.0.4. On the **Browse** tab, search for `Newtonsoft.Json`, choose version 13.0.4 from the version list, and install it.
5. Check the new version. Open `Pricing.csproj`. The `PackageReference` should show `Version="13.0.4"`.
6. Build the solution with {{Ctrl+Shift+B}}. It should finish without errors. Read the Error List and the Output window for any NuGet warning. A vulnerability warning is a reason to look at the package, not a verdict, and for 13.0.4 you should see none.

## Check your work

The project file should end with `Version="13.0.4"` for Newtonsoft.Json, and the build should succeed with no NuGet warning for it. If a warning names the package, read it and check the package's nuget.org page before you change anything else.

~~~spoiler
Here is one correct way to do the homework.

In **Manage NuGet Packages**, go to the **Installed** tab and remove Newtonsoft.Json. Check that the `PackageReference` line is gone from `Pricing.csproj`. Then, on the **Browse** tab, search for `Newtonsoft.Json`, choose version 13.0.4, and install it. Open the project file, and check that the new line reads `Version="13.0.4"`.

If the build reports a NuGet warning, read it. The version 13.0.4 is the latest stable release, so a warning about it would be unexpected. Check the package's page on nuget.org before you decide anything.
~~~

When you finish, leave the package at 13.0.4. The checklist in the next lesson keeps it there.
