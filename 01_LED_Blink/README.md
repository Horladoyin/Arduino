# LED Blink – Arduino Project

## 📖 Overview
This is the classic **Arduino "Hello World"** project — making an LED blink at regular intervals.  
It’s a great first step into learning Arduino programming and understanding how to control digital outputs.

---

## 🛠️ Components Required
- **Arduino UNO** (or compatible board)
- USB cable for uploading code
- (Optional) External LED & 220Ω resistor if not using the built-in LED

---

## ⚡ Circuit Diagram
- This project uses the built-in LED connected to **digital pin 13** on most Arduino boards.
- If using an external LED:
  1. Connect the positive leg (anode) of the LED to **digital pin 13** through a **220Ω resistor**.
  2. Connect the negative leg (cathode) of the LED to **GND**.

*(Insert `schematic.png` here once added)*

---

## 💻 Code

```cpp
// The setup function runs once at startup
void setup() {  
  pinMode(13, OUTPUT);     // Initialize digital pin 13 as an output
}

// The main loop runs repeatedly
void loop() {
  digitalWrite(13, HIGH);  // Turn the LED on
  delay(1000);             // Wait for 1 second
  digitalWrite(13, LOW);   // Turn the LED off
  delay(1000);             // Wait for 1 second
}
