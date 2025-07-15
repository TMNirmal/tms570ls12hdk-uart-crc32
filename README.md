# UART CRC32 Calculator on TMS570LS12HDK

This project implements a high-speed UART-based CRC32 calculator using the TI TMS570LS12HDK (Hercules) microcontroller. It receives data over UART and calculates the Ethernet-standard CRC32 checksum after an idle timeout period.

---

## Features

- UART communication at baud rate 937500
- Detection of idle timeout (500 ms) to finalize CRC calculation
- CRC32 calculation using Ethernet polynomial (IEEE 802.3)
- Uses SCI2 (USB UART) interface on the TMS570 board
- Suitable for embedded diagnostics and communication verification

---

## Hardware

- **Microcontroller:** TI TMS570LS12HDK Hercules series
- **Debugger:** XDS100v2 USB Debug Probe
- **Communication Interface:** SCI2 (UART over USB)

---

## Getting Started

### Prerequisites

- Code Composer Studio (CCS)
- HALCoGen (for peripheral setup)
- TI TMS570LS12HDK board
- UART terminal software (e.g., TeraTerm, PuTTY)

### Building and Flashing

1. Clone this repository:
   ```bash
   git clone https://github.com/TMNirmal/tms570ls12hdk-uart-crc32.git
