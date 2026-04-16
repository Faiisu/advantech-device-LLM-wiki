---
title: "CAN Bus"
type: concept
tags: [hardware, embedded, industrial, automotive, fieldbus, can-bus]
created: 2026-04-16
updated: 2026-04-16
sources: [ARK-1125H, ARK-1221L, ARK-1250L, ARK-3534C, ARK-3534D]
---

# CAN Bus

## Definition

Controller Area Network (CAN) — a robust serial communication protocol originally developed by Bosch for automotive applications. Allows microcontrollers and embedded devices to communicate without a host computer, using a two-wire differential bus (CAN-H, CAN-L). ISO 11898 standard.

## Why It Matters

CAN Bus is the dominant protocol in automotive ECU networks, industrial robots, medical devices, and building automation. An embedded PC with native CAN ports can directly interface with vehicle systems, motion controllers, and industrial fieldbus networks without an external CAN adapter.

## Key Properties

- **Physical layer:** differential 2-wire (CAN-H/CAN-L), terminated 120Ω at each end
- **Speed:** CAN 2.0 up to 1 Mbps; CAN FD (Flexible Data-rate) up to 8 Mbps
- **Multi-master bus:** any node can transmit; collision detection via arbitration
- **Message-based:** identified by message ID, not node address — enables broadcast
- **Error detection:** CRC, bit stuffing, ack slots — very robust in high-noise environments
- **Typical range:** up to 40 m at 1 Mbps; longer at lower speeds

## CAN in ARK Series

| Model | CAN Ports | Series Tier | Notes |
|---|---|---|---|
| [[ARK-1125H]] | 2× CAN Bus | Compact DIN-rail | Built-in |
| [[ARK-1221L]] | 1× CAN Bus | Wide DIN-rail | Built-in |
| [[ARK-1250L]] | 1× CAN Bus | Wide DIN-rail | Optional (CAN 2.0) |
| [[ARK-3534C]] | 2× CAN Bus | Expansion box PC | Feature list (not in spec table) |
| [[ARK-3534D]] | 2× CAN Bus | Expansion box PC | Feature list (not in spec table) |

CAN version (2.0A/2.0B/FD) not specified in any source spec.

## Related Concepts

[[Industrial IO]], [[Fanless Embedded PC]], [[DIN-Rail Mounting]]

## Sources

[[ARK-1125H]], [[ARK-1221L]], [[ARK-1250L]], [[ARK-3534C]], [[ARK-3534D]]
