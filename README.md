# Yagi-2Element-VHF
This repository contains the input file (2mTutorial.nec) for a simulation of a two-element Yagi antenna (Dipole + Reflector) designed for the 146 MHz VHF band.

This project shows how to design and analyze a directional antenna array built to focus the radio signal in one specific direction.
| Parameter | Value | Technical Role |
| :--- | :--- | :--- |
| **Driven Element (Active)** | 0.988 m | The main element that is fed, set near the half-wavelength ($\lambda/2$). |
| **Reflector Length (Passive)** | 1.1 m | Made **longer** than the Driven Element. This creates an inductive load, which **pushes the signal forward** (away from the reflector). |
| **Element Spacing** | 0.25 m | Controls the phase relationship between elements, optimizing the final beam shape and gain. |
| **Feed Point** | Wire 1, Segment 10 | The precise point where the 1V voltage source is applied to excite the antenna. |
| Measurement | Expected Result | **Actual Result** | Technical Insight |
| :--- | :--- | :--- | :--- |
| **Radiation Pattern** | Unidirectional | Confirmed | The pattern should show a strong main lobe pointing forward (away from the Reflector element). |
| **Peak Gain** | Higher than 2.15 dBi | **6.48 dBi** | **High Gain Achieved:** The gain is significantly higher than a simple dipole, confirming the directional effect of the reflector. |
| **Input Impedance ($Z_{in}$)** | Will change significantly | **$53.02 + j45.53 \ \Omega$** | The reflector element correctly reduced the real part ($R$), but introduced a large **imaginary part ($jX$)**, confirming the need for matching. |
| **VSWR (Ref. $50 \ \Omega$ cable)** | Low | **2.36:1** | This is a moderately high VSWR, which is common in Yagi designs and confirms that a final **matching circuit** is required before practical use. |
Conclusion: This project successfully models the design principles of a basic directive antenna array and provides clear data showing the high gain achieved through element interaction.Conclusion: This project successfully models the design principles of a basic directive antenna array and provides clear data showing the high gain achieved through element interaction.
![Uploading image.png…]()
