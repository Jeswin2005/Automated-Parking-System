# Automated-Parking-System
An Arduino-based automated parking system using ultrasonic sensors, a servo barrier, and an LCD display.

**Features**
Detects available parking slots using ultrasonic sensors.
Displays real-time parking availability on an LCD screen.
Controls a servo motor to operate the parking barrier.
Automatically updates the number of available parking slots when vehicles enter or exit.

**Components Used**
Arduino Uno
Ultrasonic Sensors (HC-SR04) - 5 units
Servo Motor
16x2 LCD Display
Jumper Wires
Breadboard

**Circuit Connections**
Component            |Arduino Pin
LCD (RS, E, D4-D7)   |12, 11, 5, 4, 3, 2

Ultrasonic Sensor 1  |10

Ultrasonic Sensor 2  |9

Ultrasonic Sensor 3  |8

Ultrasonic Sensor 4  |7

Ultrasonic Sensor 5  |13

Servo Motor          |6


**Working Principle**

**Parking Slot Detection:**

Ultrasonic sensors continuously measure the distance to check for empty or occupied slots.

If a slot is occupied, it is marked as unavailable.

**Barrier Control:**

When a vehicle is detected at the entrance and slots are available, the servo motor lifts the barrier.

When the vehicle enters, the slot count is updated, and the barrier closes.

When a vehicle exits, the slot count updates, and the barrier opens if another vehicle is waiting.

**LCD Display Output:**

Shows the number of available slots.

Indicates if parking is full.

Displays free slots dynamically.
