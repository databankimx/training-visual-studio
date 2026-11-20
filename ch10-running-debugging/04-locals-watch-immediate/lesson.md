# Locals, Watch, and Immediate windows

Three windows show you what the program is doing while it is paused. Each one is listed under Debug, then Windows, and you can open any of them from there.

- **Locals** lists the variables in the current method, with their values. It updates each time you step.
- **Watch** shows only the expressions you add. Use it for a value you want to keep an eye on, such as a total that changes inside a loop.
- **Immediate** runs code you type while the program is paused. Use it to test an expression before you change the code.

Figure 10.2 shows the debugger stopped on a line, with the Locals window open below the editor.

![Figure 10.2 - The debugger stopped with the Locals window open](images/ch10-locals.png "width=75%")

*Figure 10.2 - The debugger stopped with the Locals window open*

## Try it

1. Set a breakpoint on the first line of PriceCalculator.Total in Pricing/PriceCalculator.cs, and start with {{F5}} from PriceReport.
2. Choose Debug, then Windows, then Locals. Find the variable prices, and expand it to see the four values.
3. Press {{F10}} twice to move to the start of the loop. The loop has not run yet, so total is still 0.
4. Right-click total in the Locals window, and choose Add Watch. The Watch window shows total with the value 0, as Figure 10.3 shows, because the loop has not added anything yet. The watch stays visible as you step.

![Figure 10.3 - The Watch window with total added](images/ch10-watch-total-zero.png "width=75%")

*Figure 10.3 - The Watch window with total added, before the loop runs*

5. Press {{F10}} to run the loop once. After the first pass, total shows 12.50. Press {{F10}} until the loop has made a second pass, and total shows 20.50, as Figure 10.4 shows. Visual Studio shows the changed value in red.

![Figure 10.4 - The Watch window after two passes through the loop](images/ch10-watch-second-pass.png "width=75%")

*Figure 10.4 - The Watch window after two passes through the loop*

6. Choose Debug, then Windows, then Immediate, or press {{Ctrl+Alt+I}}. Click in the window, type `prices.Count`, and press Enter. The answer appears below it, and it is 4.

## Using the Immediate window

The Immediate window is a prompt. It stays blank until you type something, and it runs what you type only while the program is paused. Start the debugger, and let it pause at a breakpoint inside the method you want to test. Then click in the window, type an expression, and press Enter. The result appears on the next line.

The window runs real code, too. While the program is paused in Total, type `PriceCalculator.Average(prices)`, and press Enter. The method runs during the break, and the answer appears as 11.0625. The program stays paused, so you can keep stepping afterward.

Output from `Console.WriteLine` does not appear in the Immediate window. Type `Console.WriteLine(prices[0]);`, and press Enter. The Immediate window reports that the expression has been evaluated and has no value, because the method returns nothing. The number itself, 12.50, appears in the console window of the running program, as Figure 10.5 shows.

![Figure 10.5 - The Immediate window and the program's console window during a break](images/ch10-immediate-console.png "width=60%")

*Figure 10.5 - The Immediate window and the program's console window during a break*

Stepping through the method first helps, because the variables you can see in the Locals window are the ones you can use in the Immediate window. If you type a name and get an error, check that the program is paused, and that the name exists at that line.

## Common mistake

The Locals window shows only the variables in the current method. To see variables in the method that called it, open the Call Stack window with Command Search, type Call Stack, and choose the calling frame.
