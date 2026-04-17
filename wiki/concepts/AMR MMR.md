---
title: "AMR MMR"
type: concept
tags: [amr, mmr, robotics, autonomous, mobile-robot, industrial]
created: 2026-04-17
updated: 2026-04-17
sources: [MIC-760, mic-7000-series-overview]
---

# AMR MMR

## Definition

AMR (Autonomous Mobile Robot) refers to robots that navigate independently using onboard sensors, maps, and path planning — without requiring fixed tracks or infrastructure changes. MMR (Material Movement Robot) is a variant or sub-category focused specifically on autonomous material transport within factories, warehouses, and logistics facilities.

## Why It Matters

AMR/MMR systems require a highly integrated compute platform combining real-time processing (motion control, sensor fusion), high-bandwidth connectivity (camera/LiDAR data), industrial communication (EtherCAT, CANbus, Modbus), and wireless networking — all in a compact, rugged package. This distinguishes the compute requirements from standard factory automation PCs.

## Key Properties

- Navigation relies on sensor fusion: LiDAR, cameras, IMUs, wheel encoders
- Multiple Ethernet ports required for simultaneous camera/LiDAR/network connections
- Wireless: fast-roaming WiFi (target ≤50ms handoff) essential for continuous operation across access point coverage zones
- CANbus and EtherCAT used for motor drives, servo controllers, and actuators
- ROS2 is the dominant middleware for AMR/MMR software stacks
- Compact form factor required to fit within robot chassis
- Isolation on I/O ports important due to noisy motor drive environments

## Evidence and Examples

- [[MIC-760]]: purpose-built AMR/MMR controller with 3× GbE (camera/LiDAR), 4× USB 3.2, CANbus, isolated DIO, serial ports, 36ms WiFi fast roaming, ROS2 package
- MIC-760 targets CTOS (Configure-To-Order) robot system integrators who need a validated Linux+ROS2 stack on Advantech hardware

## Tensions and Contradictions

- No ARK-series model in this wiki is positioned for AMR/MMR; the MIC-760 fills a gap the ARK line does not address (mobile, WiFi, ROS2).

## Related Concepts

[[ROS2]], [[CAN Bus]], [[EtherCAT]], [[Industrial IO]], [[Fanless Embedded PC]]

## Sources

[[MIC-760]], [[mic-7000-series-overview]]
