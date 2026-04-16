---
title: "Industrial IO"
type: concept
tags: [hardware, embedded, industrial, serial, io]
created: 2026-04-16
updated: 2026-04-16
sources: [ARK-6322]
---

# Industrial IO

## Definition

The set of communication interfaces and signal lines used to connect an industrial computer to field devices — sensors, PLCs, actuators, barcode scanners, displays, and other industrial equipment. Distinct from consumer I/O (HDMI, USB-C) in that it prioritizes reliability, distance, noise immunity, and legacy compatibility over bandwidth.

## Key Interface Types

| Interface | Notes |
|---|---|
| **RS-232** | Point-to-point serial; up to ~15m; most common legacy COM port |
| **RS-422** | Differential, longer distance (~1200m), one transmitter |
| **RS-485** | Differential, multi-drop (up to 32 devices on one bus); dominant in industrial fieldbus |
| **GPIO** | General-purpose digital I/O; used for triggers, status signals, relay control |
| **Gigabit Ethernet** | Standard networking; also used for industrial protocols (Modbus TCP, EtherNet/IP) |

## ARK-6322 I/O Profile

The ARK-6322 provides a strong industrial I/O set:
- 6x COM ports (5x RS-232 fixed, 1x RS-232/422/485 software-selectable)
- 8x USB (1x USB 3.0, 7x USB 2.0)
- 2x GbE
- 8-bit GPIO
- 2x Mini PCIe for optional expansion (WWAN, WLAN)

The 6-COM profile suggests use cases with multiple serial field devices (e.g., POS systems, machine control, SCADA terminals).

## Related Concepts

[[Fanless Embedded PC]], [[iDoor]], [[Mini PCIe]]

## Sources

[[ARK-6322]]
