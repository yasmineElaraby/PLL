# 3.2 GHz Charge-Pump PLL Design

## Overview
This project implements a **charge-pump phase-locked loop (CHP-PLL)** designed to generate a stable **3.2 GHz output** from a **25 MHz reference**.  
The design targets low phase noise, minimal reference spurs, and fast lock time for high-speed RF/mixed-signal applications.

---

## Main Specifications

| Parameter                | Value              | Notes                                   |
|--------------------------|--------------------|-----------------------------------------|
| **Reference Frequency**  | 25 MHz             | Crystal oscillator or low-jitter source |
| **Output Frequency**     | 3.2 GHz            | Synthesized via integer-N division      |
| **Architecture**         | Charge-Pump PLL    | Integer-N                                |
| **Divider Ratio (N)**    | 128                | Fout = Fref × N                          |
| **Phase Detector Type**  | PFD (D flip-flop)  | Sequential with tri-state output         |
| **PFD Frequency**        | 25 MHz             | Equals reference frequency               |
