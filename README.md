# Attenuation Measurement -Limited Fiber Length 2.5 GB & 10 GB
# NAME : SHIYAM KUMAR S 
# REG NO : 212223060260
## Objective
- Calculate the attenuation-limited fiber length based on the power budget equation.  
- Simulate the resulting system and verify that it meets performance objectives.
---
## Theory
The **power budget equation** states that the power budget in a transmission system must equal the sum of all power losses plus the power margin.  
The power budget is the difference between the transmitter output power and the receiver sensitivity in dBm:
<img width="994" height="468" alt="image" src="https://github.com/user-attachments/assets/28074fe1-e571-4356-bf4c-29cf212c8173" />
In this exercise, all parameters are given except the fiber length, which must be determined.  
The **receiver sensitivity** is defined as the minimum power required to achieve a BER of <img width="54" height="38" alt="image" src="https://github.com/user-attachments/assets/56f53e67-161a-4d53-ba6e-e31a3725ea43" />, corresponding to a Q factor of 6.  
- Receiver sensitivity depends on the bit rate.  
- Fiber attenuation depends on the operating wavelength.  
---
## Pre-lab Calculations
Using the power budget equation and the parameters below, determine the attenuation-limited fiber length:
- **Transmitter output power:** 0 dBm  
- **Operating wavelength:** 1550 nm  
- **Bit rate:** 2.5 Gb/s  
- **Receiver sensitivity:** -30 dBm  
- **Fiber attenuation:** 0.19 dB/km  
- **Number of connectors:** 2  
- **Loss per connector:** 0.5 dB  
- **Additional known losses:** 0 dB  
- **Power margin:** 6 dB
---
## Layout
- The system has been created using **OptiSystem** and exported as an **OptiPerformer** file.  
- Two versions exist: one for **2.5 Gb/s** and one for **10 Gb/s**.  
- Work with the **2.5 Gb/s** version first.  
- An optical attenuator represents connector loss and system margin.  
- Adjust parameters according to the table above.  
- Dispersion and nonlinear effects in the fiber are disabled.  
- To set the receiver sensitivity to -30 dBm for 2.5 Gb/s, set the **thermal noise parameter** in the receiver to **8.97e-24 W/Hz**.  
- Visualizer components are included to obtain necessary simulation data.  
---
## Simulation
1. Run the simulation and record:
   - **Optical power levels (dBm):**
     - Both ends of fiber  
     - Receiver input  
   - **BER analysis:**
     - BER  
     - Q factor  
     - Eye diagram  
2. Set the fiber length to **125% of the calculated pre-lab value** and repeat the simulation and data recording.  
---
## Analysis and Report
# CALCULATION 
<img width="1394" height="1423" alt="exp 2 original 1" src="https://github.com/user-attachments/assets/f937ca4a-c9e9-43c4-9fa3-47c250edd253" />
<img width="1059" height="1600" alt="exp 2 original 2 " src="https://github.com/user-attachments/assets/f4c061d9-f5d4-48bb-ac28-c20c45259b35" />
# 2.5 GB 
<img width="1600" height="900" alt="EXP 2 2 5 GB" src="https://github.com/user-attachments/assets/7dcc5498-da5f-4808-ac70-6a6be77eb8e3" />
# 10 GB 
<img width="1600" height="900" alt="EXP 2   10GB" src="https://github.com/user-attachments/assets/79f954a8-0ce8-4fd2-8360-73a6e8f790ef" />
## Result
Thus the attenuation-limited fiber lenght based on the power budget equation is successfully simulated and verified.



