# Find in Files

Find in Files searches the text of every file in the solution at once. Use it when you know a word, a method name, or a message appears somewhere in the code, but you do not know which file it is in. It is the fastest way to answer a question such as where is this value used?

## Starting a search

Press {{Ctrl+Shift+F}}. The Find in Files box opens. Type the text you want to find, and press {{Enter}}. The matches appear in a Find Results window, grouped by file.

Try it with the word Total. The practice solution uses that word in three projects, so the results list matches in more than one file.

Figure 4.2 shows the Find Results window with matches from the practice solution.

![Figure 4.2 - Find in Files results for the word Total](images/ch04-find-in-files-results.png "width=75%")

*Figure 4.2 - Find in Files results for the word Total*

## Reading the results

Each line in the results shows the file name, the line number, and the line of text that matches. Scroll through the list to see every match. Double-click a line to open that file at the exact line, with the match selected. That makes it easy to move from a result to the code and back.

## Options

Under the search box are a few options, and they change what counts as a match.

- **Match case** makes the search care about capital letters, so Total does not match total.
- **Match whole word** finds only complete words, so a search for Total does not match Totals.
- **Use regular expressions** lets you describe a pattern rather than a fixed word. Leave it off for now.
- **Look in** controls where the search runs. Set it to Entire Solution for this lesson.

## Find in Files or Find?

Find in Files covers the whole solution. To search only the file you have open, press {{Ctrl+F}} instead. That opens the Find box, which works inside one file and moves between matches in that file.

## Try it

1. Press {{Ctrl+Shift+F}}, type Total, and set Look in to Entire Solution.
2. Press {{Enter}}, then count the matches in each file.
3. Double-click the match in PriceReport/Program.cs. The file opens at that line.
4. Press {{Ctrl+Shift+F}} again, turn on Match whole word, and search for Total. Compare the number of matches with the first search.
