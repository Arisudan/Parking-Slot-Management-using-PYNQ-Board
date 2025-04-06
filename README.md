# Parking Slot Management System

## Overview

This project presents a Verilog-based simulation of a **Parking Slot Management System**. In modern smart parking lots, sensors detect vehicle entry and exit to manage available slots. This simulation replicates that concept using push buttons to mimic vehicle movement in and out of the parking lot. A Seven Segment Display (SSD) is used to show the number of currently available parking spaces.

This project is ideal for learners looking to understand digital logic design, Verilog HDL, and simulation-based verification of simple embedded systems.

---

## Key Features

- Simulates a functional parking slot management system
- Entry and exit controlled using push buttons
- Real-time display of available parking slots using SSD
- Supports dynamic increment and decrement operations
- Ideal for beginner to intermediate Verilog developers
- Easily extendable to real-world sensor-based parking systems

---

## Hardware Simulation Setup

This project is intended to run in a simulation environment and does not interface with real hardware. However, it can be extended to hardware platforms such as FPGAs with appropriate I/O mapping.

---

## Components and Modules

| Component             | Functionality Description                                                                            |
|-----------------------|------------------------------------------------------------------------------------------------------|
| Entry Button          | Simulates vehicle entry. Each press reduces the available slot count by one                         |
| Exit Button           | Simulates vehicle exit. Each press increases the available slot count by one                        |
| Slot Counter Register | Holds the current number of free parking slots                                                      |
| Seven Segment Display | Outputs the number of available slots in real-time                                                  |
| Control Logic         | Verilog logic that updates the slot counter and drives the SSD display based on input conditions    |

---

## How the System Works

1. **Initialization**
   - The system starts with a predefined number of free slots.
   - This number can be configured in the Verilog code.

2. **Entry Simulation**
   - When the entry button is pressed, the system assumes a vehicle has entered.
   - The available slot count is decremented by one.
   - The new count is reflected on the SSD.

3. **Exit Simulation**
   - When the exit button is pressed, the system assumes a vehicle has left.
   - The available slot count is incremented by one.
   - The SSD updates accordingly.

4. **Overflow/Underflow Handling**
   - The system can be designed to ignore additional entries when the lot is full (i.e., slot count = 0).
   - Similarly, exit inputs can be ignored when the lot is already empty (to avoid exceeding total capacity).

---

## Simulation Instructions

### Prerequisites

- A Verilog simulation tool such as:
  - ModelSim
  - Vivado Simulator
  - Icarus Verilog
  - EDA Playground (for online simulation)
- Basic understanding of Verilog and digital design

### Steps

1. Clone or download the repository.
2. Open the project in your simulation tool of choice.
3. Compile all Verilog source files.
4. Run the testbench or interact with buttons via waveform tools or simulation inputs.
5. Observe the output on the simulated Seven Segment Display.

---

## Sample Scenario

Assume the parking lot has a maximum of 5 slots.

1. Simulation starts: SSD shows `5`
2. Press Entry → SSD shows `4`
3. Press Entry → SSD shows `3`
4. Press Exit  → SSD shows `4`
5. Continue simulation to test various conditions

---

## Customization Options

- **Initial Slot Count**: Modify the initial value in the slot counter register
- **Display Logic**: Enhance SSD control for multiple digits if needed
- **Debounce Logic**: Add if using real buttons on hardware
- **Sensor Integration**: Replace buttons with sensor module inputs in FPGA implementation
- **Full Lot Handling**: Add warning signals or messages when the lot is full

---

## Potential Enhancements

- Add buzzer or LED indicators for full or empty status
- Integrate with UART or LCD for detailed display
- Expand to handle multiple parking zones or levels
- Implement using Finite State Machines (FSM) for more control logic clarity

---

## Files Included

- `parking_system.v`: Main Verilog module for the parking logic
- `ssd_driver.v`: Seven Segment Display driver module
- `testbench.v`: Testbench for simulating the design
- `README.md`: This documentation file

---

## Contribution

This repository is created and maintained by **Arisudan**. Contributions are welcome to improve functionality, add hardware support, or expand the project scope.

To contribute:

1. Fork this repository
2. Create a new branch for your feature
3. Commit your changes
4. Submit a pull request

Issues, bug reports, or suggestions can be submitted via GitHub Issues.

---

## License

This project is open-source and available under the MIT License. You are free to use, modify, and distribute with proper attribution.

---
🤝 Contribute
This repository is maintained by Arisudan.
Contributions, suggestions, and improvements are always welcome!

Fork the repo • Create a feature branch • Submit a pull request 🚀

---
### Author: [ARISUDAN TH]
GitHub: [https://github.com/Arisudan]
