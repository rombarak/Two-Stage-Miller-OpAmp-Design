# Two-Stage Miller Operational Amplifier Design

## Project Overview
This repository presents the design, simulation, and optimization of a Two-Stage Miller CMOS Operational Amplifier, implemented in Cadence Virtuoso.

The project focuses on achieving high open-loop gain, robust stability, and optimal bandwidth through careful transistor sizing and classical Miller frequency compensation, while comparing theoretical design formulas with post-layout simulation behavior.

---

## Key Specifications & Performance

| Parameter | Value |
|---------|-------|
| Open-Loop Gain | 72.07 dB |
| Phase Margin (PM) | 62.94° |
| Unity Gain Bandwidth (UGB) | ~2.14 MHz |
| Supply Voltage | 1.8 V |
| Bias Current (Iref) | 2 µA |
| Output Load Capacitance | 1 pF |
| Miller Compensation Capacitor | 2.5 pF |

Phase margin exceeds the 60° stability target.  
Bias current selected to ensure sufficient voltage headroom.

---

## Architecture & Design Highlights

- Topology
  - NMOS differential input pair
  - Common-source second gain stage

- Frequency Compensation
  - Miller capacitor inserted between the first-stage output and second-stage input
  - Enables pole-splitting and improves closed-loop stability

- Optimization Process
  - Iterative simulations across multiple Miller capacitor values
  - 2.5 pF chosen as the optimal trade-off between phase margin, bandwidth, and settling behavior

- Theory vs. Practice
  - Classical Sansen-based formulas used as a baseline
  - Adjustments required due to short-channel effects and modern CMOS non-idealities

---

## Analysis Performed

### DC Analysis
- Verified correct biasing and operating points
- Robust saturation region observed between 632 mV and 1.79 V

### Transient Analysis
- Step response evaluated for multiple Cmiller values
- Comparison between underdamped and overdamped responses

### AC / Frequency Analysis
- Bode magnitude and phase plots
- Extraction of open-loop gain, unity-gain frequency, and phase margin

---

## Documentation

A full technical report is included with:
- Schematics
- Simulation setups
- Parameter sweeps
- Theoretical derivations
- Result interpretation

Two stage Miller Amp.pdf  
`./Two%20stage%20Miller%20Amp.pdf`

---

## Tools Used

- Cadence Virtuoso – Schematic capture
- Spectre / Maestro – Simulation and analysis
- ViVA – Waveform visualization and measurement

---

## Key Takeaways

- Complete analog IC design flow from theory to simulation
- Stability-driven design decisions in low-power operational amplifiers
- Clear illustration of the gap between textbook models and real CMOS behavior
