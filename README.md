# STM32F103 Custom Control Board (PCB Project)

This project is a **custom-made PCB (Printed Circuit Board)** built around the **STM32F103C8T6 microcontroller**.  
The goal of this project was to learn how to design a **real hardware board** instead of only using ready-made development boards.

This board can be used for **sensor reading, communication, and embedded control applications**.

---

## 🎯 Project Goal

To design a working STM32 board that includes:

- Stable power supply
- Communication ports (CAN, UART, I2C)
- Debugging support
- A PCB that is ready for manufacturing

---

## 🧠 Main Components Used

| Part | What it Does |
|------|---------------|
| STM32F103C8T6 | Main microcontroller (the brain of the board) |
| CAN Transceiver | Allows CAN communication (used in robotics & industry) |
| UART Header | Used for serial communication and debugging |
| I2C Pins | Used to connect sensors |
| SWD Pins (SWIO, SWCLK) | Used to upload and debug firmware |
| Capacitors | Reduce noise and stabilize power |
| Voltage Regulation | Provides safe voltage to MCU |

---

## 🔧 What I Added Beyond the Tutorial

This board was inspired by Phil’s Lab STM32 tutorial, but I added extra features:

| Feature | Why I Added It |
|---------|----------------|
| CAN Communication | Used in industrial and robotic systems |
| Extra UART Access | Easy debugging and data output |
| I2C Support | To connect sensors |
| Better Debug Header | Easy firmware upload and testing |

---

## ⚡ Power Design (Simple Explanation)

- Small capacitors placed near MCU to reduce noise
- Bigger capacitors used to keep voltage stable
- Ground plane used to make signals cleaner

---

## 🧩 PCB Design Steps I Followed

1. Created the schematic (circuit diagram)
2. Chose the components
3. Placed components on PCB
4. Checked 3D view to see board shape
5. Routed connections
6. Ran DRC (error check)
7. Generated Gerber files
8. Prepared BOM list

---

## 🧪 How the Board Can Be Tested

If powering the board for the first time:

1. Check voltage using multimeter
2. Check clock signal
3. Upload firmware using ST-Link and SWD pins
4. Test UART communication on PC
5. Check I2C sensor connection
6. Test CAN communication

---
