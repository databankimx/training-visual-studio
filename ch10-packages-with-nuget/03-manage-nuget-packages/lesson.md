# Adding a package with Manage NuGet Packages

Visual Studio has a window for packages. It lists the packages a project uses, searches nuget.org, and shows the version each package can be updated to. This lesson adds Newtonsoft.Json at version 13.0.3, so the next lessons have a version to change.

## Open the window

In Solution Explorer, right-click the `Pricing` project, and choose **Manage NuGet Packages**. The window opens with three tabs:

- **Browse** searches for a package on the feed and installs it.
- **Installed** lists the packages the project already uses, and removes them.
- **Updates** lists packages that have a newer version.

## Add the package

1. On the **Browse** tab, search for `Newtonsoft.Json`.
2. Choose the result with that exact name, and check that its publisher is the one you judged in the last lesson.
3. In the version list on the right, choose **13.0.3**. The newest version is selected by default, so you must change it.
4. Choose **Install**. Visual Studio may show a **Preview Changes** dialog that lists what it will add. Read it, then choose **Apply**.
5. Wait for the window to finish. The package appears on the **Installed** tab.

The package's code is now available to `Pricing`. The `Pricing` code doesn't use it yet, and that is fine.

## What the window changed

Open `Pricing.csproj` from Solution Explorer. A new `ItemGroup` holds a `PackageReference` for `Newtonsoft.Json`, with `Version="13.0.3"`. The window wrote that line. The next lesson shows how to read it and change it yourself.

## Try it

1. Right-click `Pricing`, and choose **Manage NuGet Packages**.
2. On **Browse**, search for `Newtonsoft.Json`, choose version 13.0.3, and install it.
3. Open `Pricing.csproj`, and find the `PackageReference` line. Check that its version is 13.0.3.

The Package Manager Console also installs packages, with a command such as `Install-Package`. It is the older route, and this course uses the window, because it shows the package's details as you choose.
