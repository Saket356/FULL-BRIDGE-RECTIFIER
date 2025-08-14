# FULL-BRIDGE-RECTIFIER
# Full Bridge Rectifier using MOSFETs in LTspice ⚡

This project implements and simulates a **Full Bridge Rectifier** using four NMOS transistors in **LTspice XVII**.  
The simulation includes gate drive pulses, an AC input source, and load analysis to study waveform behavior and efficiency.

## Overview 📘

The circuit:
- Uses **four IRF7455 NMOS** transistors in an H-bridge configuration
- Driven by complementary gate pulses (`Vg1` and `Vg2`)
- Converts an AC input into a DC output across a resistive load
- Includes transient simulation to capture waveform transitions

**Outputs observed:**
- **AC Input Voltage** waveform
- **Rectified DC Output** waveform
- **Gate Pulses** driving the MOSFETs (ensuring switching sequence)

## Tools Used 🛠️

- **LTspice XVII** – Circuit simulation
- **IRF7455 MOSFET Model** – Power NMOS transistor
- **SINE Source** – AC input
- **PULSE Sources** – MOSFET gate drive signals

## Key Highlights ✅

- Demonstrated AC-to-DC conversion using MOSFETs instead of diodes
- Simulated input, output, and gate drive waveforms
- Identified that gate pulses must be timed properly to avoid overlap (shoot-through)
- Showcased transient switching characteristics

## How to Run 🚀

1. Clone or download this repository  
2. Open the `.asc` schematic file in LTspice  
3. Run the `.tran` simulation command  
4. Use the probe tool to plot:
   - **Input waveform** (AC source)
   - **Output waveform** (across load resistor)
   - **Gate drive pulses** (`Vg1` and `Vg2`)
5. Verify that gate pulses do not overlap to prevent cross-conduction

## Folder Structure 📂

