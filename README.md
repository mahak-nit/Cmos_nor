# CMOS NOR Gate Implementation Using Tanner EDA

Project Overview:
This project demonstrates the implementation and simulation of a CMOS NOR gate using Tanner EDA tools. The CMOS structure is designed in S-Edit, the SPICE netlist is written in T-Edit, and the output waveform is analyzed in W-Edit to verify the logic operation.

Objective:
To design and simulate a CMOS NOR gate and verify its functionality using input and output waveforms.

Tools Used:
- S-Edit: To design the CMOS NOR gate transistor-level structure.
- T-Edit: To write the SPICE netlist for simulation.
- W-Edit: To analyze the simulated waveforms and verify the NOR gate operation.

Logic Function:
The Boolean expression for a two-input CMOS NOR gate is:
Y= ~(A+B)
Where: A, B:Input signals
       Y:Output signal

CMOS Circuit Design:
The CMOS NOR gate consists of:
Two PMOS transistors connected in series in the pull-up network.
Two NMOS transistors connected in parallel in the pull-down network.
The output becomes HIGH only when both inputs are LOW. If either input is HIGH, the output becomes LOW.

Implementation Steps:
1. S-Edit: Draw the transistor-level CMOS NOR gate circuit using two PMOS transistors in series and two NMOS transistors in parallel.
2. T-Edit: Write the SPICE netlist describing the transistors, input voltage sources, power supply, and transient analysis.
3. Simulation: Run the simulation to generate the output data.
4. W-Edit: Open the simulation results and plot the input signals (A and B) and output signal (Y).
5. Verification: Compare the output waveform with the NOR gate truth table to confirm correct operation.

Truth Table:
|  A  |  B  |  Y  |
|  0  |  0  |  1  |
|  0  |  1  |  0  |
|  1  |  0  |  0  |
|  1  |  1  |  0  |

Waveform Verification:
The simulated waveforms in W-Edit are used to verify the NOR gate operation.
- When A = 0 and B = 0, the output Y = 1.
- When A = 0 and B = 1, the output Y = 0.
- When A = 1 and B = 0, the output Y = 0.
- When A = 1 and B = 1, the output Y = 0.
The output waveform should be HIGH only when both inputs are LOW, confirming the NOR gate's functionality.

Result:
The CMOS NOR gate is designed in S-Edit, simulated using a SPICE netlist in T-Edit, and verified by analyzing the input and output waveforms in W-Edit.

Key Learning Outcomes:
- Understanding CMOS pull-up and pull-down networks.
- Implementing a NOR gate using PMOS and NMOS transistors.
- Writing a SPICE netlist for circuit simulation.
- Analyzing transient waveforms to verify digital logic functionality.
