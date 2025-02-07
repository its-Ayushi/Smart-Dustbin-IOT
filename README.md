
# Smart Dustbin Using Arduino

This project demonstrates how to create a **Smart Dustbin** using **Arduino Uno**, an **Ultrasonic Sensor (HC-SR04)**, and an **SG90 Micro Servo Motor**. The dustbin automatically opens its lid when it detects an object (such as a hand) within a specified distance, and the lid stays open for a few seconds before closing automatically.

## Components Required

- **Arduino Uno** (1)
- **Ultrasonic Sensor (HC-SR04)** (1)
- **SG90 Micro Servo Motor** (1)
- **9V Battery** (1)
- **Dustbin** (1)
- **Jumper Wires** (1 set)
- **Double-Sided Tape** (for mounting components)

## Software Required

- **Arduino IDE** (Download from [Arduino official website](https://www.arduino.cc/en/software))

## Circuit Diagram

Here is a basic outline of the connections:

- **Ultrasonic Sensor (HC-SR04)**:
  - VCC -> 5V on Arduino
  - GND -> GND on Arduino
  - Echo -> Pin 6 on Arduino
  - Trig -> Pin 5 on Arduino
- **SG90 Micro Servo Motor**:
  - VCC -> 5V on Arduino
  - GND -> GND on Arduino
  - Signal Pin -> Pin 7 on Arduino
- **Arduino Uno**:
  - Power via 9V Battery connected to the **Vin Pin**

## Working

The smart dustbin uses the ultrasonic sensor to detect objects within a specific distance. When an object comes closer (less than 50 cm, by default), the servo motor opens the dustbin lid for 3 seconds. After the set time, the lid automatically closes. 

You can modify the detection distance and time duration by adjusting the parameters in the code.

## Setup and Installation

### Step 1: Connect the Components
1. Connect the ultrasonic sensor to the Arduino as described in the Circuit Diagram.
2. Mount the servo motor on the dustbin and connect it to the Arduino.
3. Attach the Arduino and sensor inside the dustbin using double-sided tape.

### Step 2: Upload the Code
1. Open the **Arduino IDE** on your computer.
2. Copy and paste the code from `smart_dustbin.ino` into the Arduino IDE.
3. Select your Arduino board and the correct COM port in the **Tools** menu.
4. Upload the code to the Arduino.

### Step 3: Power the Project
- Use a **9V battery** to power the Arduino and the connected components.
- Your **Smart Dustbin** will now be ready to use!


## Troubleshooting

- **Servo motor not working**: Make sure the servo motor is properly connected to pin 7. Also, ensure that your power supply is sufficient.
- **Ultrasonic sensor not detecting**: Ensure the sensor is properly connected to the correct pins (Trig to 5 and Echo to 6).
- **Distance too short/long**: Adjust the threshold distance (50 cm) in the code if needed.


