<div align="center">

# Intel 8086 Microcomputer System

**A complete educational microsystem built around the Intel 8086, combining hardware design and low-level assembly programming**

![CPU](https://img.shields.io/badge/CPU-Intel%208086-blue?style=flat-square)
![Language](https://img.shields.io/badge/Language-Assembly%208086-green?style=flat-square)
![Design](https://img.shields.io/badge/Design-EasyEDA-orange?style=flat-square)
![Peripherals](https://img.shields.io/badge/Peripherals-8251%2C%208255%2C%208253-purple?style=flat-square)

</div>

---

## 1. Overview

This project implements a **complete microcomputer system** based on the **Intel 8086 microprocessor**, designed for educational purposes.

It combines **hardware design (EasyEDA)** with **low-level software development (8086 Assembly)**, providing a full understanding of how classic computing systems are structured and operated.

---

## 2. System Architecture

The microsystem is built around the **Intel 8086 microprocessor** and integrates memory, I/O interfaces, and peripherals through dedicated address decoding logic.

### Central Processing Unit
- Intel 8086 acts as the core of the system
- Responsible for instruction execution and coordination of all components

### Memory Subsystem
- **EPROM (27C2048)** – stores program code (non-volatile)
- **SRAM (62512)** – used for runtime data (volatile)
- Memory is accessed through proper address mapping and decoding

### Input / Output Interfaces
- **8251 USART**
  - Enables serial communication (data transmission and reception)

- **8255 PPI**
  - Provides programmable parallel I/O
  - Used to interface with keypad, LEDs, and display

### Timer
- **8253 Programmable Interval Timer**
  - Generates timing signals
  - Used for delays and synchronization

### Input Device
- **4×3 Matrix Keypad**
  - Scanned using row-column technique
  - Detects user input via polling

### Output Devices
- **LEDs** – controlled via 8255 ports

- **6-Digit 7-Segment Display**
  - Multiplexed display system
  - Continuously refreshed using timed routines

### Interconnection
- Components are connected using:
  - Address decoding logic
  - Control signals (RD, WR)
  - Data and address buses

- Entire system designed and simulated in **EasyEDA**

### Software Layer
- Implemented in **8086 Assembly**
- Modular subroutines handle:
  - Initialization
  - Input processing
  - Display control
  - Communication
  - Timing operations

---

## 3. Features

- Full **Intel 8086-based system**
- Memory interfacing (EPROM + SRAM)
- Serial communication via **8251**
- Parallel communication via **8255**
- Programmable timing with **8253**
- Matrix keypad scanning
- LED control
- 6-digit multiplexed 7-segment display
- Modular assembly implementation

---

## 4. System Flow

1. **Initialization**
   - Configure memory and peripherals

2. **Input Handling**
   - Scan keypad and detect pressed keys

3. **Processing**
   - Execute logic using assembly routines
   - Manage timing via 8253

4. **Output**
   - Update LEDs
   - Refresh 7-segment display

5. **Communication**
   - Handle serial data via USART

---

## 5. Technologies Used

| Category     | Components / Tools |
|--------------|------------------|
| CPU          | Intel 8086       |
| Language     | 8086 Assembly    |
| Design       | EasyEDA          |
| Memory       | 27C2048, 62512   |
| Interfaces   | 8251, 8255       |
| Timer        | 8253             |
| I/O Devices  | Keypad, LEDs, 7-Segment |

---

## 6. Project Structure

```bash
.
├── hardware/        # EasyEDA schematics
├── assembly/        # 8086 Assembly code
├── docs/            # Documentation (Romanian)
└── README.md
