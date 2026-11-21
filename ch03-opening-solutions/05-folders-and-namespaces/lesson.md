# Folders and namespaces

A folder in a project groups related files, and the Solution Explorer shows it with a folder icon. Creating one is quick. Right-click the project, choose Add, then New Folder, and type a name.

A folder does not change the code in the files it holds, but Visual Studio does use it when it creates a new file. The namespace of the new file is built from the project's default namespace and the folder's path. The default namespace for Pricing is Pricing, which is why every file in the course starts with namespace Pricing;. A class added to a folder named Discounts gets the namespace Pricing.Discounts.

The namespace controls how other code refers to the class. Code in a different namespace needs a using line to reach it, or the full name:

```csharp
using Pricing.Discounts;

decimal total = Coupons.Apply(prices);
```

Two cautions. Visual Studio sets the namespace only when it creates a file, so if you move a file into a folder later, check its namespace line yourself. The compiler also does not require the folder and the namespace to match, so a mismatch builds, although Visual Studio may suggest a fix.

## Try it

1. Right-click Pricing, choose Add, then New Folder, and name the folder Scratch.
2. Right-click Scratch, choose Add, then Class, and name it Sample.
3. Read the first lines of Sample.cs, and find the namespace. It should read Pricing.Scratch.
4. Right-click Scratch, and choose Remove or Delete, so the practice solution is back to how it was.
