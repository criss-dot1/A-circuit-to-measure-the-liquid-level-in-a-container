# My first project
## Description:
The project aims to create an electronic circuit capable of monitoring the liquid level in a container using a resistive sensor and optical indicators (LEDs)

The system uses a sensor whose resistance varies linearly with the liquid level, in a range of 30kΩ – 45kΩ, corresponding to a depth of up to 230 cm. The circuit is powered at 13V and uses voltage comparators to activate LEDs of different colors depending on the thresholds reached
## Components:
### Operational Amplifier: 
- LM124

### Sensor: 
- Resistive transducer (linear variation)

### LEDs: 
  - yellow (LA_T676): Low level (< 80 cm)

  - orange (LO_3336): Medium level (80 – 180 cm) 

  - red (LU_5351): High level (> 180 cm)
### Resistors: 
- Precision series E96 (1% tolerance) and E24 (5% tolerance)
## PSpice Analysis and Simulations:
The project includes a verification of the circuit operation through several important analyses:

### Time Domain (Transient) & Parametric Sweep Analysis:
Verification of the circuit behavior and the switching thresholds for the LEDs
### Monte Carlo Analysis:
Statistical evaluation of the circuit for 310 simulations, taking into account the tolerances of the components 

V(out) min: 9.41V 

V(out) max: 12.31V
### Worst Case Analysis:
Determination of the behavior under the most unfavorable conditions (e.g.: decreasing the nominal values ​​by 10%)
## Design Calculations:
The system is based on voltage divider connected to  non-inverting amplifier
### Sensor Resistance Calculation ($R_s$): 
Determined by linearity formula for 80 cm ($35.21k\Omega$) and 180 cm ($41.73k\Omega$) thresholds
### Reference Voltages:
Calculated to ensure accurate switching thresholds at $10.66V$ and $11.82V$





