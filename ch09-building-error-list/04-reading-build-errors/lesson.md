# Reading a list of build errors

A build can report many errors for one mistake. The compiler reads the code from the top of the file to the bottom, and once it hits a mistake, it sometimes cannot make sense of the lines that follow. Those lines then report errors that would go away if the first one were fixed. Reading the list in the right order saves you from chasing errors that do not need fixing.

## Start at the first real error

Find the error that appears earliest in the file. A missing semicolon, a missing brace, or a misspelled keyword is a common first error, and it often causes several more on the lines below it.

Fix that error, then build again. Several of the others usually disappear with it.

## Read each message

Each error has a code, such as CS1002 for a missing semicolon, and a message that describes the problem. The message names the thing the compiler could not find or could not use, such as a name that does not exist. Read the message before you change the code, because the fix depends on what it says.

## Warnings and errors

Errors stop the build. Warnings do not, but they often point to a real problem, such as a variable that is declared and never used. Fix the errors first, then read the warnings and decide which ones need action.

## Try it

1. Open PriceReport/Program.cs. Add a new line at the end of the file that reads `Console.WriteLine("Done")`
2. Press {{Ctrl+Shift+B}}. Open the Error List, and read the first error. It reports a missing semicolon.
3. Add the semicolon at the end of the line, and build again. The error count drops.
4. Press {{Ctrl+Z}} as many times as needed to remove the line, and save the file.

## Common mistake

Fixing the last error in the list first is a common habit, and it wastes time. The last error is often a result of an earlier mistake, so it may disappear on its own.
