# Adding items to a project

A project grows by adding files, folders, and references to other projects. Right-click a project in the Solution Explorer, and choose Add. Figure 3.4 shows the menu for the Pricing project.

![Figure 3.4 - The Add menu on a project in the Solution Explorer](images/ch03-add-menu.png "width=40%")

*Figure 3.4 - The Add menu on a project in the Solution Explorer*

Four items on this menu do most of the work:

- **New Item** (Ctrl+Shift+A) opens a dialog with file templates, such as Class, Interface, and Text File. Choose a template, type a name, and Visual Studio creates the file in the project and opens it.
- **Existing Item** (Shift+Alt+A) copies a file from your disk into the project. Use it when the file already exists outside the project.
- **New Folder** creates a folder inside the project, to group related files. The next lesson explains how a folder affects the code inside it.
- **Class...** creates a new class file. It is a quicker route to the Class template in New Item, and the usual choice when you need only a class.

The Project Reference item connects one project to another. Pricing.Tests already has a project reference to Pricing, which is how its tests call PriceCalculator.

## Try it

1. Right-click Pricing in the Solution Explorer, and choose Add.
2. Find New Item, Existing Item, and Class, and read their shortcuts.
3. Press {{Ctrl+Shift+A}} to open the New Item dialog, look at the templates, and press Cancel. Nothing is added.
