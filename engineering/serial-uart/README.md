# UART Implementation

### Goal
I would like for my FPGA to communicate with my PC. 

### Solution
Develop a UART module to enable serial communication.

### UART Background
Before writing the code, I must understand how the UART module should function.

1. Two wires between transmitter and receiver to communicate in both directions.
2. Asynchronous - receiver and transmitter do not share a common signal. However, they must transmit at the same speed, have the same frame structure and parameters.
