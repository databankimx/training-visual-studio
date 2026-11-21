# 10. Packages with NuGet

A package is a library that someone else wrote and published, so your project can use it without copying its code. NuGet is the package system for .NET, and nuget.org is the public place where most packages live. This chapter adds one well-known package, Newtonsoft.Json, to the `Pricing` project in the practice solution, and it shows two ways to do that: the Manage NuGet Packages window, and a direct edit of the project file.

Most of the work is judgment. Before a package goes into a project, you read its page, check its license and owners, and decide whether it belongs there. The window is the easy part.

> **Before you start:** the Manage NuGet Packages window works without a sign-in. Visual Studio's account and license are covered in Chapter 2. Every example in this chapter uses packages from nuget.org.

## Your organization's packages

Your organization may run a private NuGet feed, on its own authenticated GitHub Enterprise instance. Reaching a private feed needs a sign-in, and the rules for it, and for which packages are approved, belong to your organization. This course doesn't use a private feed, and it doesn't give any address or credentials for one. If you work for an organization, follow its rules for private feeds and approved packages, and ask your team which ones apply before you add anything.

## What the chapter covers

The chapter has seven lessons, from the basics to the checklist:

1. What a package is, and how a project refers to one.
2. How to judge a package on its nuget.org page before you add it.
3. Adding a package with the Manage NuGet Packages window.
4. Editing the package reference in the project file.
5. Homework: removing a package, then adding it back at a new version.
6. A checklist.
7. A summary with three quizzes.

The practice project is `Pricing` in `training-visual-studio-practice`. It has no packages yet, so you can see exactly what each step adds.

---
