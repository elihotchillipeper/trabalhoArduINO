# INSTALATION
1. **Setting up the Development Environment:** Make sure you have a development environment set up for Arduino programming. This includes having the Arduino IDE installed on your computer. If you haven't installed the Arduino IDE yet, you can download it for free from the official Arduino website and follow the installation instructions for your operating system.

2. **Open the Arduino IDE:** After installing the Arduino IDE, open the program.

3. **Create a New Sketch:** In the Arduino IDE, click on File > New to create a new sketch.

4. **Copy and Paste the Code:** Copy the provided code and paste it into the Arduino IDE editor, replacing the default sketch content.

5. **Verify and Compile the Code:** Before uploading the code to the Arduino, click on the verify button (checkmark icon) at the top of the IDE to check for any syntax errors in the code.

6. **Connect the Arduino:** Connect your Arduino to the computer using a USB cable.

7. **Select the Board and Port:** Go to Tools > Board and select the type of Arduino board you are using (e.g., Arduino Uno).
Then, go to Tools > Port and select the COM port to which the Arduino is connected.

8. **Upload the Program:** Click on the upload button (right arrow icon) in the top left corner of the IDE to compile and upload the program to the Arduino.

9. **Verify Execution:** Once the upload is successfully completed, the program will run on the Arduino. You can verify the output using LEDs or other hardware connected to the pins configured in the code.

By following these steps, you will be able to install and run the program on your Arduino smoothly. Ensure to adjust physical connections as needed, especially if using LEDs or other output devices configured on the Arduino pins.

# USAGE
### Using the Software:
1. **Connection and Setup:** Connect the bits of sets nib1 and nib2 to input pins (0 to 7) and output pins (8 to 12) for sum results and carry bit. Upload the code onto the hardware using the Arduino IDE.

2. **Start of Operation:** The program waits for a signal on pin 13 to begin binary addition.

3. **Sum Processing:** When the signal on pin 13 is received (sum == 1), it calculates the bit sum using specific functions for each bit and updates the carry bit.

4. **Output of Results:** The sum results and carry bit are sent to output pins 8 to 12, ready for use by other devices or circuits.

5. **Continuous Execution:** The program repeats these steps continuously, waiting for a new signal on pin 13 to start a new addition operation.
