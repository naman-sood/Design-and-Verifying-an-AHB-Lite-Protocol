# Design-and-Verifying-an-AHB-Lite-Protocol
AHB-Lite based bus system designed and verified using SystemVerilog. Implemented master-slave communication, address decoding, burst transfers, and wait-state handling. Developed verification scenarios for single/burst read-write operations, invalid address accesses, back to back transactions, and data integrity testing. 


# AHB-Lite Bus System Design and Verification

## Overview

This project focuses on the design and verification of an AHB-Lite based bus system using Verilog/SystemVerilog. The system was developed to understand AMBA AHB-Lite protocol behavior, on-chip communication, and hardware verification methodologies.

The project includes implementation of bus components such as master, slaves, address decoder, and interconnect logic, along with a structured verification environment to validate protocol functionality under multiple scenarios.

---

## Features

* Single Read and Write Transactions
* Burst Transfers (4-beat, 8-beat, 16-beat)
* Wait State Handling
* Back-to-Back Transactions
* Address Decoding Logic
* Default Slave/Error Response Handling
* Read-Only Access Protection
* Data Integrity Verification
* Verification Scenarios for Edge Cases

---

## Project Structure

```text
├── rtl/                # RTL design files
├── tb/                 # Testbench files
├── simulation/         # Simulation outputs/waveforms
├── docs/               # Reports and documentation
└── README.md
```

---

## Verification Scenarios

The system was tested using multiple verification scenarios including:

| Scenario ID | Description               |
| ----------- | ------------------------- |
| S1          | Single Write              |
| S2          | Single Read               |
| S3          | Read-Only Write Attempt   |
| S4          | Invalid Address Access    |
| S5          | Wait State Write          |
| S6          | Wait State Read           |
| S7          | 4-Beat Burst Write        |
| S8          | 8-Beat Burst Write        |
| S9          | 16-Beat Burst Write       |
| S10         | 4-Beat Burst Read         |
| S11         | 8-Beat Burst Read         |
| S12         | Back-to-Back Transactions |
| S13         | Slave Selection           |
| S14         | Back-to-Back Read         |
| S15         | Back-to-Back Write        |
| S16         | Data Integrity Check      |

---

## Tools and Technologies

* Verilog / SystemVerilog
* ModelSim / Vivado (depending on your simulator)
* Digital Design and Verification Concepts
* AMBA AHB-Lite Protocol

---

## Learning Outcomes

Through this project, we gained practical understanding of:

* Bus architecture and communication protocols
* RTL design methodology
* Hardware verification flow
* Debugging protocol-level timing and response issues
* Importance of corner-case and stress testing

One of the biggest takeaways was learning that successful verification is not just about making the design work, but ensuring it behaves correctly under unexpected conditions.

---

## Team

Developed by:

* Naman Sood
* Akshat Tripathi

Under the guidance of faculty members at Jaypee Institute of Information Technology.

---

## Future Improvements

* UVM-based verification environment
* Functional coverage implementation
* Randomized transaction generation
* Protocol compliance automation
* Multi-master AHB support

---

## License

This project is intended for educational and academic purposes.
