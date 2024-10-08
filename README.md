## Task 24: Microwave Oven Timer Application

#### Overview
This task involves designing a typical **Microwave oven timer** using the **4x4 keypad** and **16x2 LCD** present on the STC development kit. The microwave timer will implement features such as start/pause, door safety switch, and buzzer notifications.

#### Instructions

1. **Keypad Input for Timer:**
   - Use the **4x4 keypad** to enter the time for which the microwave should run.
     - The entered time (in minutes/seconds) should be displayed on the **16x2 LCD** with a **Hitachi HD44780 driver**.

2. **Start/Pause Functionality:**
   - The oven should **start** or **pause** by pressing the **ON** key on the keypad.
   - If the oven is paused, pressing the **ON** key again will resume operation from where it left off.

3. **Clearing Timer:**
   - The **= key** should clear the time entered on the keypad, resetting the display on the LCD.

4. **Safety Door Switch:**
   - Incorporate a **door switch** to ensure user safety.
     - **Opening the door** should immediately stop the oven.
     - After **closing the door**, the oven can be resumed by pressing the **ON** key.

5. **Buzzer Notifications:**
   - Use a **buzzer** to indicate different events:
     - **Short beeps** for key presses.
     - **Long beep** for time-out (when the timer reaches zero).
     - **Warning beep** if there's any error or unsafe condition (e.g., the door is open while trying to start the oven).

6. **Controlling the Microwave Magnetron:**
   - Use an **electromagnetic relay** to control the power of the **magnetron**.
     - The relay should be turned **on** when the microwave is running and **off** when it is paused, stopped, or when the door is open.

7. **State Machine Implementation:**
   - Implement the entire program using a **finite state machine** (FSM).
     - Possible states can include:
       - **Idle** (waiting for input).
       - **Running** (oven is heating).
       - **Paused** (oven is temporarily stopped).
       - **Door Open** (safety mode, oven stopped).
       - **Time Out** (when the timer reaches zero).

8. **Additional Features:**
   - Optional: You can add any other features you think might enhance the final product, such as:
     - Power level adjustment.
     - Timer display in countdown format (MM:SS).
     - Visual indicators like LEDs for additional feedback.

9. **Final Product Example:**
   - Watch this [video](https://www.youtube.com/watch?v=oVj2MSlzRCo&ab_channel=ChipSoulTechnology%28SMCPrivate%29Limited) for an example of how the final product might look.
   - Feel free to add your own creative modifications or enhancements based on the example in the video.

---
