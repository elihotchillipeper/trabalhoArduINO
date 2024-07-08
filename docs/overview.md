# OVERVIEW

This software implements an Arduino program to perform binary addition of 4-bit numbers. Here's an overview of its main features and functionality:

#### Initial Variables
- `int soma = 13;`: Controls the start of the addition operation when reading the state of pin 13.
- `int carryBit = 0;`: Stores the carry bit during the addition operation.
- `int nib1a, nib1b, nib1c, nib1d = 0;`: Variables that store the individual bits of the first 4-bit binary number (`nib1`).
- `int nib2a, nib2b, nib2c, nib2d = 0;`: Variables that store the individual bits of the second 4-bit binary number (`nib2`).
- `int res1a, res1b, res1c, res1d = 0;`: Variables that store the results of the addition for each corresponding bit (`res1`).

#### **fullAdder** Function
- Implements the logic of a full adder, essential for adding individual bits.
- Parameters:
  - a, b: Input bits for addition.
  - cIn: Input carry bit.
  - sum: Reference to store the sum result.
  - cOut: Reference to store the carry out result.
- Computes the sum (sum) and determines the carry out (cOut) based on the inputs.

#### Setup
- Configures the Arduino pins:
  - Pins 0 to 7 as inputs to read the input binary numbers (`nib1` and `nib2`).
  - Pins 8 to 12 as outputs to display the results of the binary addition (`res1` bits and `carryBit`).
  - Pin 13 as input to initiate the addition process (`soma`).

#### Main Loop
- Reads the state of pin 13 (`soma`) to determine when to start the binary addition.
- Reads the individual bits (`nib1` and `nib2`) from the corresponding input pins.
- If `soma` equals 1, initializes `carryBit` to 0 and uses the `fullAdder` function to add the individual bits (`nib1` and `nib2`), storing the results in `res1` and updating `carryBit`.
- Updates the output pins (8 to 12) with the addition results (`res1` bits and `carryBit`).

### Functionality
This program is ideal for educational purposes, demonstrating practically how to perform basic binary arithmetic operations using an Arduino. It showcases the use of functions, pin control, and binary addition logic, providing a valuable introduction to digital electronics and embedded programming concepts.
