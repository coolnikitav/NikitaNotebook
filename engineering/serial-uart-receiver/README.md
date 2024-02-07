# UART Receiver

## Initial design

### Goal
I would like for my FPGA to receive data from my PC. 

### Solution
Develop a UART module to enable serial communication.

### UART Background
Before writing the code, I must understand how the UART receiver module should function.

1. Two wires between transmitter and receiver to communicate in both directions.
2. Asynchronous - receiver and transmitter do not share a common signal. However, they must transmit at the same speed, have the same frame structure and parameters.

### Design
I will design a UART with 1 start bit, 8 data bits, 1 odd parity bit, and 1 stop bit.

### Code
[uart.v](https://github.com/coolnikitav/nikitas-notebook/blob/main/engineering/serial-uart/uart.v)

[parity.v](https://github.com/coolnikitav/nikitas-notebook/blob/main/engineering/serial-uart/parity.v)

### Testing
[testbench](https://github.com/coolnikitav/nikitas-notebook/blob/main/engineering/serial-uart/uart_tb.v)

[waveforms](https://github.com/coolnikitav/nikitas-notebook/blob/main/engineering/serial-uart/uart_tb_waveform.md)

### Analysis
The UART module successfully receives messages.

## FPGA Integration

Now, since the UART module is successfully receiving sample messages during testing, I will adjust it to work with my Basys 3 FPGA.

The [Basys-3-Master.xdc] constraints file indicates that the FPGA is receiving data through pin B18:

##USB-RS232 Interface
set_property -dict { PACKAGE_PIN B18   IOSTANDARD LVCMOS33 } [get_ports RsRx]

B18 will be the data bit.
