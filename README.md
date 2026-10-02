# Automatic-Rain-Sensing-Wiper
Hardware-based automatic rain-sensing wiper system using 555 Timer, LM358, and L293D motor driver.

An automated vehicle windscreen wiper system that detects rainfall via a custom-etched rain sensor and drives a DC motor back and forth to clear moisture[cite: 5, 6]. 

## 🛠️ Components & Hardware Stack
* **IC Timer:** 555 Timer IC (configured in Astable Multivibrator mode)[cite: 6]
* **Comparator:** LM358 Operational Amplifier[cite: 6]
* **Motor Driver:** L293D IC[cite: 6]
* **Transistor:** BC557 PNP Transistor (acts as main power switch)[cite: 7]
* **Sensor:** Custom-built rain/water detector (fabricated using a copper-clad board and Ferric chloride etching solution)[cite: 6, 7]
* **Actuator:** DC Wiper Motor (5V-12V supply)[cite: 6, 7]

## 📋 Circuit Architecture & Working
1. **Rain Detection:** When water droplets fall on the custom rain sensor, it triggers the BC557 PNP transistor, turning ON the main power supply to the circuit[cite: 7].
2. **Pulse Generation:** The 555 timer operates in astable mode to generate periodic clock pulses[cite: 6].
3. **Control Logic:** The LM358 comparator evaluates the timer output against a reference voltage set by a voltage divider network[cite: 7].
4. **Motor Drive:** The L293D motor driver processes the alternating high/low signals to drive the DC motor clockwise and anticlockwise, sweeping the wiper left and right until the sensor surface dries[cite: 7].

## 📂 Repository Structure
* `/schematics` - Circuit diagrams and layout references.
* `Project_Report.pdf` - Complete documentation and group project report.
