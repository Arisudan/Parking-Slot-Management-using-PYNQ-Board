# 🚗 Parking Slot Management System

## 📝 Overview

This is a simple Verilog project that simulates a **parking slot management system**. Instead of real sensors, we use buttons to mimic the **entry** and **exit** of vehicles. The system keeps track of available parking slots and displays the number of free slots on a **Seven Segment Display (SSD)**.

---

## 🔧 Key Features

- Simulates vehicle **entry and exit** using buttons  
- Tracks the number of **free parking slots**  
- Displays the count on a **Seven Segment Display**  
- A great project for learning **Verilog basics**  

---

## 🧩 Components Used

| Component            | Description                                                  |
|----------------------|--------------------------------------------------------------|
| **Entry Button**     | Simulates a vehicle entering ➝ Decreases slot count         |
| **Exit Button**      | Simulates a vehicle leaving ➝ Increases slot count          |
| **Free Slot Counter**| Displays the current number of free slots on the SSD        |

---

## ▶️ How to Use

### 1. Set Up the Simulation
- Use a Verilog simulation tool like **Vivado**, **ModelSim**, etc.
- Add and compile the project files.

### 2. Run the Simulation
- Start the simulation environment.
- Initialize with a desired number of free parking slots.
- Use:
  - **Entry button** ➝ Slot count decreases
  - **Exit button** ➝ Slot count increases
- The SSD will reflect the updated slot count.

---

## 💡 Example Walkthrough

1. Start the simulation  
2. Set initial free slots (e.g., 5)  
3. Press **Entry** ➝ Slots: 4  
4. Press **Entry** again ➝ Slots: 3  
5. Press **Exit** ➝ Slots: 4  
6. Continue simulating as needed  

---

## 📌 Notes

- You can change the initial number of slots in the code.  
- While this demo uses buttons, real-world systems can use IR sensors, RFID, or cameras.

---

## 🤝 Contribute

This repository is created and maintained by **Arisudan**.  
Feel free to fork this project, suggest improvements, or open an issue.  
Your contributions are welcome!

---
