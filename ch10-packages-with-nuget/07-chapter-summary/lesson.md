# Chapter summary

Adding a package is a decision and a change to the project file. The decision comes first. The window or a hand edit records it. Keep these in mind:

- Read the package's page before you add it: the stable version, the license, the owners, the dependencies, and when it was last updated.
- A package is referenced by a `PackageReference` line in the project file, with an `Include` for the name and a `Version` for the version. Restore downloads it at the next build.
- Manage NuGet Packages has three tabs: **Browse** to find and install, **Installed** to remove, and **Updates** to see newer versions.
- You can edit a `Version` by hand, or remove a line. The window is safer, but the file is what the build reads, so check the result on the **Installed** tab.
- A vulnerability warning is a reason to look at the package, not a verdict.
- NuGet.Config sets where packages come from. Your user file is `%AppData%\NuGet\NuGet.Config`, a closer file wins for single settings, and a malformed file is ignored silently.
- Every example uses nuget.org. A private feed belongs to your organization, and its rules come first.

```quiz
Where does Visual Studio record that a project uses Newtonsoft.Json?
○ In the NuGet cache, which holds downloaded packages.
→ The cache holds downloads. It isn't where the project records its choice.
◉ In a PackageReference line in the project file.
→ Right. The build reads the PackageReference, and restore downloads the version it names.
○ In the solution's .vs folder.
→ The .vs folder holds your editor state. The package reference belongs in the project file.
```

```quiz
You want to change a package to a new version, and you edit the Version in the project file. What should you do next?
○ Nothing, because the file is saved.
→ The file is saved, but the window and the build should agree with it. Check the result.
◉ Check the version on the Installed tab, and read any restore error at the next build.
→ Right. The Installed tab shows what the project asks for, and restore reports a version it cannot find.
○ Delete the whole ItemGroup, so Visual Studio starts again.
→ Deleting the group removes every package in it. Change only the Version value you mean to change.
```

```quiz
Why does this course pin a version in every example?
○ Because nuget.org does not allow an unpinned reference.
→ nuget.org allows both. Pinning is a choice the course makes.
◉ So the output stays the same when newer versions are published.
→ Right. A pinned version gives the same result for every reader.
○ Because the newest version never works with .NET 10.
→ There is no such rule. The course pins versions to keep its steps steady.
```

---
