# The Build menu and Build Solution

The Build menu holds the commands that compile the solution. Build Solution, with {{Ctrl+Shift+B}}, compiles every project in the solution, and rebuilds only what has changed since the last build. It is the command you will use most often.

Choose Build, then Build Solution, to see the same command by name. The menu also holds Rebuild Solution, which compiles everything again from the beginning, and Clean Solution, which deletes the output of the last build. Use Rebuild when you suspect the output is out of date, and Clean when you want to remove the old files before a build.

## Try it

1. Open the practice solution. Press {{Ctrl+Shift+B}}.
2. Watch the status bar at the bottom of the window. It shows the build progress, and then the result.
3. Open the Output window with Command Search, and type Output. The Output window lists each project as it builds, and it ends with a line that counts the errors and warnings.
4. Choose Build, then Rebuild Solution. The Output window shows the whole solution compiled again.

## Reading the result

A successful build ends with a count of zero errors. The Output window shows the count of warnings too. A warning does not stop the build, but it is a sign that something may be wrong, so read each one before you move on.

## Building one project with Ctrl+B

Ctrl+B builds the current project only, not the whole solution. A developer often has most of the solution built already, and is changing just one project. In that case, Ctrl+B saves time, because it compiles only the project you are working on.

That saving has a risk. If the project you changed is used by another project, a change to a name or a method can break the other project. Ctrl+B does not build that other project, so the break stays hidden until you build the solution. Build the whole solution with Ctrl+Shift+B before you finish a change.

## Try it

1. Open Pricing/PriceCalculator.cs. In the declaration of MinPrice, type over the name so it reads MinimumPrice. Type the change by hand. Do not use Rename, because Rename would update every caller.
2. Press {{Ctrl+B}}. The Pricing project builds, because its own code is consistent.
3. Press {{Ctrl+Shift+B}}. Errors appear in PriceReport/Program.cs and in the test file, because both still call MinPrice.
4. Press {{Ctrl+Z}} to restore the name, and press {{Ctrl+Shift+B}} again to build the solution.

## Common mistake

Building only compiles the program. A successful build means the code compiles. To run the program, press {{F5}}, which Chapter 10 covers.
