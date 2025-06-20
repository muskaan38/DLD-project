# DLD-project
# Digital Logic Design Project – Code Lock

## 🔒 Project Title
**Code Lock** – A Digital Combinational Security System

## 📌 Introduction
The **Code Lock** is a hardware-only digital security system designed using basic logic gates without microcontrollers or programming. It compares a user-entered 4-bit binary code with a preset secret combination using **XNOR**, **AND**, and **NOT** gates to determine if access is granted or denied.

## 🎯 Project Vision
The goal is to build a low-cost, easily replicable electronic lock using fundamental combinational logic. This project offers hands-on experience in digital logic design and is ideal for electronics or computer engineering students to understand real-world applications of logic gates.

## 🛠 Circuit Design Overview
- **Input**: 8-bit DIP switch  
  - First 4 switches (A–D): Preset code  
  - Last 4 switches (E–H): User input  
- **Logic**:  
  - Each user input is compared with the preset bit using **IC 4077 (XNOR gates)**.  
  - The XNOR outputs are combined with an **IC 7408 (AND gate)**.  
  - If all match, a **green LED** turns ON.  
  - If mismatch, output is inverted using **IC 7404 (NOT gate)** to light up a **red LED**.

## 🧰 Components Required
| Component                  | Quantity | Description                             |
|---------------------------|----------|-----------------------------------------|
| 8-bit DIP Switch          | 1        | For code input                          |
| IC 4077 (XNOR)            | 1        | For bit-by-bit comparison               |
| IC 7408 (AND)             | 1        | To validate full code match             |
| IC 7404 (NOT)             | 1        | To indicate access denial               |
| Green LED                 | 1        | Access granted indicator                |
| Red LED                   | 1        | Access denied indicator                 |
| 220-ohm Resistors         | 2        | For LED current limiting                |
| 4.7k-ohm Resistors        | 4        | Pull-down for DIP switches              |
| 9V Battery + Clip         | 1        | Power source                            |
| 830-pin Breadboard        | 1        | For circuit assembly                    |
| Jumper Wires              | —        | For connections                         |

## ⚙️ Working Principle
1. User sets the secret code and input via DIP switch.
2. IC 4077 compares each pair using XNOR logic.
3. If all XNORs are HIGH, IC 7408 allows the green LED to light up.
4. If any bit mismatches, output goes LOW, and the IC 7404 turns on the red LED.

## ⚠️ Safety Measures
- Use current-limiting resistors for LEDs.
- Ensure DIP switch inputs are pulled down to avoid floating states.
- Avoid exceeding voltage ratings of ICs.
- Disconnect power when not in use.

## 📈 Educational Outcomes
This project enhances understanding of:
- Combinational logic
- Hardware design without software
- Digital security system basics
- Practical use of XNOR, AND, NOT gates

## 🔧 Future Enhancements
- Use of microcontrollers (e.g., Arduino) for dynamic codes
- LCD display for feedback
- Buzzer for incorrect attempts
- PCB-based compact design

## ✅ Conclusion
The **Code Lock** is a simple yet effective representation of how digital logic circuits can be implemented in practical applications. It's an excellent learning project for students and hobbyists looking to deepen their understanding of hardware-based security solutions.

---

