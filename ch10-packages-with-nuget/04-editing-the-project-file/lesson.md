# Editing the package reference in the project file

The project file is plain XML, so you can also change a package by editing it. Each package is a `PackageReference` line with two attributes: `Include` names the package, and `Version` names the version the project asks for. The window writes this line, and you can read it, change it, or remove it yourself.

```xml
<ItemGroup>
  <PackageReference Include="Newtonsoft.Json" Version="13.0.3" />
</ItemGroup>
```

## Change the version

To change a version by hand, edit the `Version` value in `Pricing.csproj`, and save the file. If Visual Studio offers to reload the project, accept. Then open **Manage NuGet Packages** on the **Installed** tab, and check that the window shows the new version.

Restore runs at the next build. A version that doesn't exist on the source fails at that point, with an error that names the package and the version. Read the error before you change anything else.

## Remove a line by hand

To remove a package by hand, delete its `PackageReference` line. An empty `ItemGroup` can stay or go, and both work. The **Installed** tab's remove action does the same job, and it avoids a typo in the package name.

## Why the window is safer

The window checks that the package exists before it writes the line, and it writes the line in the format the tools expect. Use a hand edit when you want to see or change a single value, and check the result on the **Installed** tab either way.

Some organizations set package versions in one central file, so each project refers to a version set elsewhere. If the solution has a `Directory.Packages.props` file, the `Version` is set there, and the project's line has no `Version` attribute. Check that file before you edit a version in the project.

## Try it

1. Open `Pricing.csproj`, and find the `PackageReference` line for `Newtonsoft.Json`.
2. Change its `Version` to 13.0.4, and save the file.
3. Open **Manage NuGet Packages** on the **Installed** tab, and check that it shows 13.0.4.
4. Change the `Version` back to 13.0.3, save, and check the window again. The homework starts from 13.0.3.
