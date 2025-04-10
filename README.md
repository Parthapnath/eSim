Bistable Multivibrator using 555 Timer
A simple implementation and simulation of a Bistable Multivibrator circuit using a 555 Timer IC, built and tested using eSim and ngspice.

📜 Abstract
This project focuses on the design and simulation of a Bistable Multivibrator using a 555 Timer. Unlike astable and monostable circuits, the bistable multivibrator toggles its output based on external trigger and reset inputs, not capacitor charging/discharging. It maintains its output state until it receives another input.

🛠️ Theory and Working
The 555 Timer's trigger (pin 2) and reset (pin 4) pins are pulled HIGH via resistors R1 and R2.

Two push-button switches are connected to ground:

Pressing Trigger (S1) → Output goes HIGH.

Pressing Reset (S2) → Output goes LOW.

The output remains in its state until another input is applied.

Threshold pin (pin 6) is left open or grounded to prevent undesired switching.

⚙️ Components Used
555 Timer IC

Resistors (R1, R2)

Push-button switches (S1, S2)

Power supply (VCC, GND)

Multimeter (for monitoring output)

eSim software (for simulation)

ngspice (for waveform analysis)

🔥 Circuit Diagram
(Circuit schematic included in the repository under circuit_diagram/ folder or as PDF.)

Main Points:

Connect pins 2 and 4 to VCC via pull-up resistors.

Connect switches to pins 2 and 4 to pull them LOW when pressed.

Pin 6 (threshold) left open or grounded.

Output taken from pin 3.

📈 Simulation Results
Input/Output (ngspice)
Trigger input: A short LOW pulse to set output HIGH.

Reset input: A short LOW pulse to reset output LOW.

Plots are generated using ngspice simulation.

Python Plots
Further input vs output verification using Python plotting.

(Plots available inside plots/ folder.)

💡 Applications
Robotics: Changing direction when encountering obstacles.

Digital Electronics: 1-bit memory cell.

Simple control systems that require stable toggling.

📚 References
Electronics Hub: 2-Way Switch Wiring

Electronics Hub: Bistable Multivibrator using 555 Timer

CircuitBread: 555 Timer Bistable Multivibrator Configuration

Research Paper Reference:

Title: Design and Implementation of Bistable Multivibrator using 555 Timer

Journal: IOSR Journal of Electrical and Electronics Engineering (IOSR-JEEE)

Author: Md. Moyeed Abrar

Volume: 12, Issue 1 Ver. II (Jan.–Feb. 2017), Pages 22–29
