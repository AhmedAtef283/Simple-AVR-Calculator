# Simple-AVR-Calculator
This code implements a basic calculator using a microcontroller. The calculator allows the user to perform addition, subtraction, multiplication, and division operations on two 4-digit numbers entered through a keypad. The result is displayed on an LCD screen.

# Prerequisites
This code assumes the presence of the following libraries:
- "MCAL/Dio/Dio.h" - Library for microcontroller abstraction layer (MCAL) for Digital Input/Output (DIO) operations.
- "HAL/LCD/lcd.h" - Library for hardware abstraction layer (HAL) for controlling the LCD.
- "HAL/KEYPAD/KeyPad.h" - Library for HAL of the keypad.
- <util/delay.h> - Library for creating delays in the program.

# Functionality
- The code initializes the keypad and LCD.
- It displays a loading message on the LCD for a short duration to start the calculator.
- After the loading message, it displays a welcome message.
- The code enters a loop for repeating the calculation process indefinitely.
- Inside the loop, it prompts the user to enter the first number followed by an operation (+, -, /, x).
- If the user presses 'C', the code goes back to the start of the calculation loop.
- The code stores the first number and the selected operation.
- Then, it prompts the user to enter the second number.
- If the user presses '=', the code performs the calculation based on the selected operation.
- If the user presses 'C', the code goes back to the start of the calculation loop.
- The code converts the input numbers from arrays of digits to actual numbers.
- The calculation is performed based on the selected operation (+, -, /, x).
- The result is displayed on the LCD screen.
- The LCD screen is cleared after a short delay.

# How to Use
- Connect the microcontroller to the necessary hardware components, including the keypad and LCD.
- Include the required libraries and header files in the project.
- Build and upload the code to the microcontroller.
- The calculator will start after the loading message and display a welcome message.
- Enter the first number using the keypad.
- Press the desired operation (+, -, /, x).
- Enter the second number using the keypad.
- Press '=' to calculate the result.
- The result will be displayed on the LCD screen.
- To perform another calculation, press 'C' and repeat steps 5-9.
Note: This code assumes a specific keypad layout and the number of digits for the input numbers (4 digits). Modify the code accordingly if your hardware or requirements differ.

# Additional Notes
The calculate function performs the actual arithmetic calculation based on the selected operation. It converts the input numbers from arrays of digits to actual numbers and uses a switch statement to determine the operation to perform.
The variable KpValue is used to store the value of the pressed button on the keypad.
The code uses delay functions from the <util/delay.h> library to introduce delays between operations.

# Contributors
This code was developed by Team 16.
