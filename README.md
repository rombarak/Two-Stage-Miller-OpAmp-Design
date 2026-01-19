# Two-Stage Miller Operational Amplifier Design

## Project Overview
[cite_start]This repository contains the design, simulation, and optimization of a **Two-Stage Miller CMOS Operational Amplifier**, implemented using **Cadence Virtuoso**[cite: 1, 37, 72]. [cite_start]The project focuses on achieving high stability and gain through precise transistor sizing and frequency compensation using the Miller effect[cite: 14, 19, 21].

## Key Specifications & Performance
* [cite_start]**Open-Loop Gain:** 72.07 dB[cite: 165].
* [cite_start]**Phase Margin (PM):** 62.94° (Meeting the target of >60° for stability)[cite: 164].
* [cite_start]**Unity Gain Bandwidth (UGB):** Optimized at ~2.14 MHz[cite: 125, 126].
* [cite_start]**Power Supply:** 1.8V[cite: 10, 25].
* [cite_start]**Bias Current (Iref):** 2 μA, selected for optimal voltage headroom[cite: 26, 35].
* [cite_start]**Output Load:** 1 pF[cite: 16, 127].

## Design Highlights
* [cite_start]**Architecture:** NMOS differential pair input stage followed by a common-source second stage[cite: 1, 15].
* [cite_start]**Compensation Strategy:** Implementation of Miller capacitance (Cmiller) for pole-splitting and improved stability[cite: 19, 22].
* [cite_start]**Optimization:** Through iterative simulation, an optimal **2.5pF Miller capacitor** was selected to maximize bandwidth and settling time[cite: 125, 127].
* [cite_start]**Analysis:** The design compares empirical results with classical theoretical formulas (Sansen), highlighting the adjustments needed for modern short-channel transistor characteristics[cite: 78, 134, 135, 136].

## Analysis Included
* [cite_start]**DC Analysis:** Verified operating points and identified a robust saturation region between 632mV and 1.79V[cite: 43, 50].
* [cite_start]**Transient Response:** Step response characterization across various Cmiller values to analyze underdamped vs. overdamped behavior[cite: 72, 79, 139].
* [cite_start]**Frequency Analysis (Bode Plot):** Magnitude and phase characterization to verify stability margins and open-loop gain[cite: 155, 156, 162].

## Documentation
For a detailed technical breakdown, including all schematics, simulation setups, and in-depth result analysis, please refer to the full project report:
* [**Two stage Miller Amp.pdf**](./Two%20stage%20Miller%20Amp.pdf)

## Tools Used
* [cite_start]**Cadence Virtuoso** – Schematic Editor[cite: 1, 5].
* [cite_start]**Spectre / Maestro** – Simulation & Results[cite: 30, 80].
* [cite_start]**ViVA** – Waveform Analysis[cite: 37, 121].
* [cite_start]**Cadence Virtuoso** (Schematic Editor)[cite: 1, 5].
* [cite_start]**Spectre / Maestro** (Simulation & Results)[cite: 30, 80].
* [cite_start]**ViVA** (Waveform Analysis)[cite: 37, 121].
