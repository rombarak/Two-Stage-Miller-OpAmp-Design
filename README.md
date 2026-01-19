
# Two-Stage Miller Operational Amplifier Design

## Project Overview
[cite_start]This repository contains the design, simulation, and optimization of a **Two-Stage Miller CMOS Operational Amplifier**, implemented using **Cadence Virtuoso**[cite: 1, 37, 72]. [cite_start]The project focuses on achieving high stability and gain through precise transistor sizing and frequency compensation using the Miller effect[cite: 14, 19, 21].

## Key Specifications & Performance
* [cite_start]**Open-Loop Gain:** 72.07 dB[cite: 165].
* [cite_start]**Phase Margin (PM):** 62.94° (Meeting the target of $>60^\circ$ for stability)[cite: 164].
* [cite_start]**Unity Gain Bandwidth (UGB):** Optimized at ~2.14 MHz[cite: 125, 126].
* [cite_start]**Power Supply:** 1.8V[cite: 10, 25].
* [cite_start]**Bias Current ($I_{ref}$):** 2 $\mu$A, selected for optimal headroom[cite: 26, 35].
* [cite_start]**Output Load:** 1 pF[cite: 16, 127].

## Design Highlights
* [cite_start]**Architecture:** NMOS differential pair input stage followed by a common-source second stage[cite: 1, 15].
* [cite_start]**Compensation Strategy:** Utilized a Miller capacitor ($C_{Miller}$) to ensure system stability and perform pole-splitting[cite: 19, 22].
* [cite_start]**Optimization:** Through iterative simulations, a **2.5pF Miller capacitor** was found to be the optimal value[cite: 125, 127]. 
* [cite_start]**Theoretical vs. Practical:** The design compares empirical results with classical theoretical formulas (Sansen), noting that modern short-channel transistors require higher capacitance values than predicted for optimal settling time[cite: 78, 134, 135, 136].

## Analysis Included
* [cite_start]**DC Analysis:** Operating point verification and identification of the saturation region (632mV to 1.79V)[cite: 43, 50].
* [cite_start]**Transient Response:** Analysis of step response and settling time across various $C_{Miller}$ values to identify underdamped vs. overdamped behavior[cite: 72, 79, 139].
* [cite_start]**Frequency Analysis (Bode Plot):** Magnitude and phase characterization to verify stability margins in open-loop configuration[cite: 155, 156, 162].

## Documentation
For a detailed technical breakdown, including all schematics, simulation setups, and in-depth result analysis, please refer to the full project report:
* [**Two stage Miller Amp.pdf**](./Two%20stage%20Miller%20Amp.pdf)

## Tools
* [cite_start]**Cadence Virtuoso** (Schematic Editor)[cite: 1, 5].
* [cite_start]**Spectre / Maestro** (Simulation & Results)[cite: 30, 80].
* [cite_start]**ViVA** (Waveform Analysis)[cite: 37, 121].
