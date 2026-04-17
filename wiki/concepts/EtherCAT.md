---
title: "EtherCAT"
type: concept
tags: [ethercat, industrial-ethernet, motion-control, real-time, fieldbus]
created: 2026-04-17
updated: 2026-04-17
sources: [MIC-760]
---

# EtherCAT

## Definition

EtherCAT (Ethernet for Control Automation Technology) is an open, real-time Industrial Ethernet fieldbus protocol developed by Beckhoff Automation. It processes Ethernet frames on-the-fly as they pass through each slave node, achieving deterministic cycle times as low as 100μs — far below standard Ethernet latency.

## Why It Matters

EtherCAT is the dominant real-time communication protocol for motion control in modern industrial automation — particularly servo drives, stepper controllers, I/O terminals, and robot joint actuators. For AMR/MMR applications, EtherCAT enables tight real-time synchronization between the compute controller and multiple motor drives using standard Ethernet hardware.

## Key Properties

- Based on standard IEEE 802.3 Ethernet (physical layer) — uses standard GbE NICs in master mode
- Master processes frames in real-time; slaves extract/insert data as frame passes through
- Cycle times: typically 250μs–1ms for industrial motion control
- Topology: line, ring, tree — flexible cabling
- ESI (EtherCAT Slave Information) XML files define slave device parameters
- Standard: IEC 61158 Type 12, IEC 61784-2
- ROS2 integration via `ethercat_master` node allows ROS2 motion commands to translate directly to EtherCAT frames

## Evidence and Examples

- [[MIC-760]] includes ROS2 EtherCAT node support, enabling ROS2-based AMR motion control over EtherCAT without custom driver development

## Related Concepts

[[ROS2]], [[AMR MMR]], [[CAN Bus]], [[Industrial IO]]

## Sources

[[MIC-760]]
