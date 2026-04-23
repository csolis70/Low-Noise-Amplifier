# SR560-Low-Noise-Amplifier-

## Overview
This project documents the design, construction, and testing of a low-noise amplifier inspired by the SR560 preamplifier. The goal was to achieve stable high-gain amplification and experimentally verify that the circuit’s input-referred noise closely matches real-world specifications.

## Design
The amplifier consists of a two-stage architecture:
- A differential input stage for amplifying voltage differences and rejecting common-mode noise
- A second gain stage for additional amplification

The circuit was implemented on a breadboard and powered using ±10V supply rails.

## Key Challenges
Implementing a low-noise, high-gain analog circuit on a breadboard introduced several challenges:

- **Parasitic effects:** Stray capacitance and inductance caused instability and unwanted oscillations  
- **Op-amp limitations:** High-bandwidth op-amps (OP37, LT1028) were prone to oscillation in this setup  
- **Calibration:** Required careful tuning of offset and common-mode rejection (CMRR)

To address these issues, the original op-amps were replaced with the OPA227P, which is more tolerant of parasitic loading and improved overall stability.

## Results
- Achieved voltage gain ≈ 100×  
- Measured input-referred noise ≈ **4.33 nV/√Hz**  
- Performance closely matched the expected range from SR560 specifications  

## Key Takeaways
- Real-world implementations differ significantly from ideal circuit behavior  
- Breadboard parasitics can strongly affect high-frequency and low-noise circuits  
- Careful component selection and calibration are critical for stable amplification  

## Report
The full project report is available here:

[View Report](report/Low_Amp_Design_and_Analysis.pdf)

## Collaboration
This project was completed in collaboration with Enrique Lopez-Salinas.
