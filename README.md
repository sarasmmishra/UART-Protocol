This repository contains a Verilog implementation of the Universal Asynchronous Receiver Transmitter (UART) protocol. The project includes modules for both the transmitter and receiver, along with a testbench to verify the functionality.

Introduction:
The UART protocol is widely used for serial communication in embedded systems. This project demonstrates a Verilog-based implementation, including:
UART Transmitter: Serializes parallel data for transmission.
UART Receiver: Deserializes the received serial data into parallel data.

Testbench: Validates the behavior of the transmitter and receiver modules.

Features:
1. Configurable baud rate generator.
2. 8-bit data frame with 1 start bit, 1 stop bit, and no parity bit.
3. Synchronous reset for transmitter and receiver.
4. Validated through simulation with waveform results.

Implementation Details
1. UART Transmitter (transmitter.v)
Converts 8-bit parallel data into a serial data stream and adds start and stop bits for proper framing. It Includes a baud rate generator for precise timing.
2. UART Receiver (receiver.v)
It deserializes the incoming serial data stream back into parallel data and Synchronizes with the baud rate for accurate sampling.
