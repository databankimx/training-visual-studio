# Opening a solution

A solution file ends in .sln, and it lists the projects that belong together. Opening the solution opens all of them at once in the Solution Explorer, which is how Visual Studio expects you to work.

To open the practice solution, choose File, then Open, then Project/Solution. Find the training-visual-studio-practice folder, pick PracticeSolution.sln, and choose Open.

Figure 3.2 shows the File menu with Open and Project/Solution.

![Figure 3.2 - Open, then Project/Solution, in the File menu](images/ch03-open-solution-menu.png "width=75%")

*Figure 3.2 - Open, then Project/Solution, in the File menu*

```mermaid
flowchart TD
  A["You want to work on a solution"] --> B{"Does the folder hold a .sln file?"}
  B -->|Yes| C["File, Open, Project/Solution, then pick the .sln"]
  B -->|No| D["File, Open, Folder, then pick the folder"]
  C --> E["The Solution Explorer lists the projects"]
  D --> F["The Solution Explorer or File System view lists the files"]
```

## Open Folder as an alternative

Sometimes a folder has no solution file, or you only want to look at its files. Choose File, then Open, then Folder, and pick the folder. Visual Studio shows the files in the folder, but it does not know which projects belong together, so it cannot build the code as a solution. For the practice work, open the solution.

## Open Recent

Visual Studio remembers the solutions and folders you have opened. The File menu and the start window both list them, so you can reopen one without finding it again. Removing an item from the list only removes the entry. It does not delete anything on your computer.
