# Checklist: packages with NuGet

Tick each item when you have done it in Visual Studio.

- [ ] Opened `Pricing.csproj`, and found the target framework, with no `PackageReference` yet.
- [ ] Read the nuget.org page for Newtonsoft.Json, and wrote down its stable version, license, owners, and dependencies.
- [ ] Installed Newtonsoft.Json 13.0.3 from the Browse tab of Manage NuGet Packages.
- [ ] Found the `PackageReference` line in `Pricing.csproj`, and read its `Include` and `Version`.
- [ ] Changed the `Version` by hand to 13.0.4, checked it on the Installed tab, and put it back to 13.0.3.
- [ ] Removed the package from the Installed tab, and checked that its line left the project file.
- [ ] Added Newtonsoft.Json 13.0.4 back, and checked the project file.
- [ ] Built the solution, and read the Error List and Output window for NuGet warnings.
- [ ] Checked whether your organization has an approved list, and whether it covers this package.
