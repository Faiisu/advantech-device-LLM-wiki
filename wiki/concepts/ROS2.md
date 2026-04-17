---
title: "ROS2"
type: concept
tags: [ros2, robotics, amr, ethercat, modbus, ubuntu, middleware]
created: 2026-04-17
updated: 2026-04-17
sources: [MIC-760]
---

# ROS2

## Definition

ROS 2 (Robot Operating System 2) is an open-source robotics middleware framework providing a communication infrastructure, tools, and libraries for building robot software. It succeeds ROS 1 with improved real-time support, security (DDS-based communication), and multi-platform compatibility (Linux, Windows, embedded RTOS).

## Why It Matters

ROS2 is the de facto software platform for AMR (Autonomous Mobile Robot) and MMR (Material Movement Robot) development. A hardware platform with pre-validated ROS2 packages reduces integration time significantly — customers can deploy EtherCAT motor drives and Modbus sensors without writing communication drivers from scratch.

## Key Properties

- Based on DDS (Data Distribution Service) for publish/subscribe communication between nodes
- Real-time capable when combined with appropriate RTOS or Linux RT-preempt patches
- Advantech MIC-760 ROS2 package includes:
  - EtherCAT node — for real-time motion control of servo drives and actuators
  - Modbus node — for reading sensors, PLCs, and I/O modules via RS-485
- Requires Ubuntu 22.04 LTS (Humble Hawksbill distribution) or equivalent
- Advantech Edge Linux provides a hardened Ubuntu base for industrial ROS2 deployment

## Evidence and Examples

- [[MIC-760]] ships with Ubuntu 22.04 / Advantech Edge Linux and includes ROS2 package with EtherCAT and Modbus nodes
- Industrial WiFi fast roaming (36ms) on MIC-760 enables mobile ROS2 robots to maintain connectivity during movement across access point coverage zones

## Tensions and Contradictions

- No other model in this wiki (ARK or MIC-770/780/785) mentions ROS2; MIC-760 appears to be Advantech's designated AMR/MMR platform.

## Related Concepts

[[AMR MMR]], [[EtherCAT]], [[Industrial IO]], [[CAN Bus]]

## Sources

[[MIC-760]]
