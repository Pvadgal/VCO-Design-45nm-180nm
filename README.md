# Voltage-Controlled Oscillator (VCO) Using a 5-Stage Ring Oscillator

This repository contains the design and simulation results of a Voltage-Controlled Oscillator (VCO) based on a 5-stage ring oscillator in both 45nm and 180nm technologies. The purpose of this project is to compare the performance of the VCO under similar specifications in both process nodes. The design is simulated using Cadence tools, and the results highlight the frequency response of the oscillator in each technology.

# Specifications

- **Oscillator Type**: 5-Stage Ring Oscillator
- **Technologies**: 45nm and 180nm CMOS
- **Components Used**:
  - Inverters
  - Resistors
  - Capacitors
  - Buffers in the feedback loop (to promote propagation delay)
- **Control**: Voltage-controlled to adjust oscillation frequency is 2-2.5v
- ### Calculations
![design equations and component specifications]()


# Design

## 45nm Technology

In the 45nm process, the design uses a 5-stage ring oscillator with inverters, resistors, capacitors, and buffers to control the propagation delay and achieve oscillation. The layout is optimized for the smaller node, focusing on power efficiency and high-speed performance.

## 180nm Technology

For the 180nm process, a similar design approach is applied using the same component types, but adjustments are made to accommodate the larger transistor sizes and slower switching times typical of the 180nm node. The larger size allows for more reliable, albeit slower, performance.

# Results

- **Frequency in 45nm**: 0.1 GHz
- **Frequency in 180nm**: 0.3 GHz

As observed, the oscillator operates at a higher frequency in the 180nm technology compared to the 45nm technology. This is likely due to the differences in the intrinsic properties of the transistors used in each technology node, such as threshold voltage and capacitance, which affect the overall speed of the circuit.


### 180 nm Design
![180 nm Schematic](https://github.com/Pvadgal/VCO-Design-45nm-180nm/blob/b1b60e2494cc259d0a3edc7da5144bdfdb6b5c51/vco_180nm.jpg)
![180 nm Output Schematic](https://github.com/Pvadgal/VCO-Design-45nm-180nm/blob/c86529da7e5f0696c03f1e5f1f574d340e6797f5/vco_180nm_op.jpg)


### 45 nm Design
![45 nm Schematic](https://github.com/Pvadgal/VCO-Design-45nm-180nm/blob/bd210e23d81588896f4bb30e5c994c8f0554d206/vco_45nm.jpg)
![45 nm Output Schematic](https://github.com/Pvadgal/VCO-Design-45nm-180nm/blob/6092b5c03f432591a600b1ff77e07511a16664e0/vco_45nm_op.jpg)
# Conclusion

The 45nm design generates a slower frequency compared to the 180nm design. This difference in performance can be attributed to the resistor and capacitor values used in the circuit. The larger transistors in the 180nm process allow for faster switching, resulting in a higher oscillation frequency. In contrast, the smaller transistors in the 45nm process require more careful optimization of component values to achieve a comparable performance. 

To improve the speed of the 45nm oscillator, it is essential to optimize the resistor and capacitor values, as well as consider other design factors, such as transistor sizing and feedback loop adjustments. Proper circuit specification and optimization are key to achieving the desired frequency response in the 45nm process.

## How to Use
1. Review the images of the schematics provided above.
2. Use the design concepts for educational purposes or as a reference for VCO design.
3. The simulation is performed in Cadence Virtuoso.
