# Thai Baht Vending Machine Calculator
<h2>Description</h2>
This code is designed to operate a simple vending machine using a PIC 16F877 microcontroller. It can handle coins of different denominations and calculate the amount of money inserted into the machine. The program also displays the amount of money inserted and the number of coins inserted for each denomination on an LCD screen.<br><b>2017</b>
<h2>How to use</h2>
1. Set up the hardware (PIC microcontroller, LCD screen, and coin sensors) and connect them to the appropriate pins on the PIC microcontroller.<br>
2. Compile and upload the code to the PIC 16F877 microcontroller.<br>
3. Once the code is running on the PIC microcontroller, users can insert coins of different denominations (1, 5, or 10 baht).<br>
4. The program will keep track of the number of coins inserted and calculate the total amount of money inserted.<br>
5. The amount of money inserted and the number of coins inserted for each denomination will be displayed on the LCD screen.<br>
6. To reset the amount of money inserted and the number of coins inserted, press the reset button on the hardware.<br>
<h2>Code explanation</h2>
The program begins by initializing the hardware and setting up the LCD screen. The <b>'main'</b> function then enters an infinite loop where it checks for coins inserted by the user. If a coin is detected, the program updates the appropriate counter for that denomination of coin. The <b>'LCD'</b> function is called to update the LCD screen with the new values of the counters.

The <b>'LCD'</b> function takes the values of the counters and converts them to strings using the <b>'itoa'</b> function. It then uses the <b>'lcd_gotoxy'</b> and <b>'lcd_putc'</b> functions to display the values on the LCD screen. The <b>'ClearLCD'</b> function is called to clear any previously displayed values before updating the screen with the new values.
<h2>Future improvements</h2>
The current program is limited to handling coins of three different denominations. Future improvements to the program could include adding support for more coin denominations, adding the ability to dispense items based on the amount of money inserted, and improving the user interface to make it more intuitive and user-friendly.
<h2>License</h2>

This code is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
