# Yagi-2Element-VHF
This repository contains the input file (2mTutorial.nec) for a simulation of a two-element Yagi antenna (Dipole + Reflector) designed for the 146 MHz VHF band.

This project shows how to design and analyze a directional antenna array built to focus the radio signal in one specific direction.
Parameter,Description,Goal
Antenna Type,"Directional Array (one active element, one passive reflector).","To create a strong, focused unidirectional pattern."
Test Frequency,146 MHz.,This is the specific frequency where the design is optimized to operate.
Main Goal,To significantly increase the Gain (signal strength) compared to a simple dipole.,
Parameter,Value,Technical Role
Driven Element (Active),0.988 m,"The main element that is fed, set near the half-wavelength (λ/2)."
Reflector Length (Passive),1.1 m,"Made longer than the Driven Element. This creates an inductive load, which pushes the signal forward (away from the reflector)."
Element Spacing,0.25 m,"Controls the phase relationship between elements, optimizing the final beam shape and gain."
Feed Point,"Wire 1, Segment 10",The precise point where the 1V voltage source is applied to excite the antenna.

Measurement,Expected Result,Actual Result,Technical Insight
Radiation Pattern,Unidirectional,Confirmed,The pattern shows a strong main lobe pointing forward (Gain analysis below confirms direction).
Peak Gain,Higher than 2.15 dBi,6.48 dBi,"High Gain Achieved: The gain is significantly higher than a simple dipole, confirming the directional effect of the reflector."
Input Impedance (Zin​),Will change significantly,53.02+j45.53 Ω,"The reflector element correctly reduced the real part (R), but introduced a large imaginary part (jX), confirming the need for matching."
VSWR (Ref. 50 Ω cable),Low,2.36:1,"This is a moderately high VSWR, which is common in Yagi designs and confirms that a final matching circuit is required before practical use."
Conclusion: This project successfully models the design principles of a basic directive antenna array and provides clear data showing the high gain achieved through element interaction.
