# 💡 Moore FSM Sequence Detector — 1011 (Overlapping)

## 🧩 Overview
This project demonstrates the design and implementation of a **Moore Finite State Machine (FSM)** that detects the binary sequence **`1011`**. Unlike the Mealy FSM, the **Moore FSM** output depends **only on the current state**, providing stable and predictable output timing. This design supports **overlapping sequence detection**, where consecutive sequences can share bits.
The FSM is written in **Verilog HDL**, simulated using **Xilinx ISE Design Suite**, and verified on an **FPGA Trainer Kit**.



---

## 🎯 Project Objectives

| Objective No. | Description |
|----------------|-------------|
| 1 | Design a Moore FSM to detect the binary sequence `1011`. |
| 2 | Simulate and verify FSM functionality using **Xilinx ISE Tools**. |
| 3 | Analyze **RTL schematic**, **functional simulation**, and **synthesis reports**. |
| 4 | Implement the FSM on an FPGA Trainer Kit and verify sequence detection. |

---

## ⚙️ Hardware / Software Requirements

| Category | Tool / Component | Description |
|-----------|------------------|-------------|
| **Software** | Xilinx ISE Design Suite | Used for FSM design, simulation, and synthesis |
| **Hardware** | FPGA Trainer Kit | Used for implementation and testing |
| **Language** | Verilog HDL | Hardware Description Language used for modeling |
| **Simulation Type** | Functional Simulation | To verify sequence detection and output timing |

---

## 🧠 Theory Summary

A **Finite State Machine (FSM)** is a sequential circuit that transitions between defined states based on inputs and clock signals.  

| FSM Type | Output Depends On | Remarks |
|-----------|------------------|----------|
| **Mealy Machine** | Current **state** + **input** | Output changes immediately with input |
| **Moore Machine** | Only current **state** | Output is stable until next state transition |

In this project, a **Moore FSM** is implemented for the detection of the sequence `1011` with overlapping capability.

---

## 🔄 Design Description

| Parameter | Description |
|------------|-------------|
| **Input Signal** | `x` — Input bit stream |
| **Clock Signal** | `clk` — Synchronizes FSM transitions |
| **Reset Signal** | `reset` — Initializes FSM to default state |
| **Output Signal** | `z` — Goes high when sequence `1011` is detected |
| **Number of States** | 5 (S0–S4) |
| **Overlapping** | Supported |

---

## 🧪 Workflow

| Step | Description |
|------|-------------|
| **1. FSM Design** | Define 5-state Moore FSM for `1011` detection. |
| **2. Coding** | Implement FSM logic and testbench using Verilog HDL. |
| **3. Simulation** | Verify functional correctness in Xilinx ISE simulator. |
| **4. Synthesis** | Generate RTL schematic and timing reports. |
| **5. FPGA Implementation** | Upload bitstream and test on FPGA hardware. |

---

## 📊 Results Summary

| Test Condition | Expected Output | Observed Output |
|----------------|-----------------|-----------------|
| Input Sequence = `1011` | `z = 1` | ✅ Correct |
| Other Inputs | `z = 0` | ✅ Correct |
| Continuous Stream (`1011011`) | Overlapping detection successful | ✅ Verified |

**Result:**  
✅ The Moore FSM successfully detects the sequence `1011` with overlapping support.  
✅ Simulation, synthesis, and hardware results confirm proper design functionality.

---

## 📚 References
- [Finite State Machine – Wikipedia](https://en.wikipedia.org/wiki/Finite-state_machine)  
- [Mealy Machine – Wikipedia](https://en.wikipedia.org/wiki/Mealy_machine)  
- [Moore Machine – ScienceDirect](https://www.sciencedirect.com/topics/computer-science/moore-machine)

---

## 🏁 Keywords
`FSM` · `Moore Machine` · `Sequence Detector` · `Verilog HDL` · `FPGA` · `Xilinx ISE` · `VLSI`

---
