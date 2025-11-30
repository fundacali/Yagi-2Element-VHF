# Yagi-2Element-VHF
Two-Element Yagi-Uda Antenna simulation for the 2-meter VHF band (146 MHz)
Parameter,Value,What It Is,Purpose
Driven Element,0.988 m,The main active element (where the signal is fed).,Set near λ/2 for resonance.
Reflector Length,1.1 m,The passive element behind the active one.,Made longer than the Driven Element to push the signal forward.
Spacing,0.25 m,Distance between the two elements.,Controls the final beam shape and gain.
Feed Point,"Wire 1, Segment 10",Where the 1V voltage source is placed.,Excites the antenna.
Measurement,Expected Result,Actual Result,What We Learned
Pattern,Unidirectional,(Confirm with graphic),The signal should mainly go forward (away from the reflector).
The reflector successfully increased the signal strength. || Input Impedance ($Z_{in}$) | Will change significantly | [R] + j[X] $\Omega$ | The reflector always changes the impedance; this value shows how much we need to fix it. |Conclusion: This project successfully models the physical changes needed to turn a simple dipole into a directional array.
