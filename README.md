# embedded_project

anton maged
ali ashraf
abdelrahman el husseiny 

The provided code is an example of a program written in the C++ programming language using the MBED framework. It demonstrates a simple calculator application using a 7-segment display and a keypad for user input.

Here is a breakdown of the code:

1. Included Libraries:

   - The `mbed.h` library is included, which provides the necessary functions and definitions for using the MBED framework.

2. Define Pins:

   - DigitalOut objects are created to represent each segment (A-G) of the 7-segment display, using the pins D0 to D6.

   - DigitalIn objects are created to read the keypad input, using the pins A0 to A3.

3. Define Variables:

   - `input1` is an integer variable to store the first input from the user.

   - `operation` is a character variable to store the operation chosen by the user ('A' for addition or 'B' for subtraction).

   - `input2` is an integer variable to store the second input from the user.

4. Display Digit Function:

   - This function takes an integer parameter `digit` and uses a switch-case statement to map the digit to the appropriate segment outputs.

   - Each segment is controlled using the DigitalOut objects defined earlier.

5. Main Function:

   - The program enters an infinite loop.

   - Inside the loop, it waits for the user to enter the first input by checking the state of the keypad inputs using a while loop.

   - Based on which key is pressed, the corresponding value is stored in the `input1` variable.

   - The program then waits for the user to enter the operation in a similar manner.

   - Next, it waits for the user to enter the second input.

   - The program calculates the result based on the input values and the chosen operation.

   - If the user presses the fourth key on the keypad, it checks the value of `result` and displays it on the 7-segment display using the `displayDigit` function.

   - The loop then repeats, waiting for new user inputs.

Overall, this code demonstrates a basic calculator functionality using a 7-segment display and a keypad for user interaction. It reads user inputs, performs the requested operation, and displays the result on the 7-segment display.
