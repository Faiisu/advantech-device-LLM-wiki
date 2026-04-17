---
title: "MIC-7 Series Overview — High Performance Embedded Box IPC"
type: source
tags: [advantech, mic-series, edge-ai, i-module, modular-ipc]
created: 2026-04-17
updated: 2026-04-17
sources: []
---

# MIC-7 Series Overview — High Performance Embedded Box IPC

**Type:** Product Family Overview
**Author(s):** Advantech
**Date:** 2026
**Origin:** raw/MIC-series/High Performance Embedded Box IPC (MIC-7000).md

## Summary

The MIC-7 series is Advantech's family of compact modular industrial box PCs targeting Industry 4.0 edge intelligence. The series spans MIC-7700 through MIC-785, supporting Intel (6th Gen through Core Ultra Series 2) and AMD (Ryzen Embedded AM5) processors. A shared emphasis on i-Module expansion, Flex I/O, and iDoor interfaces allows flexible configuration. GPU expansion via i-Modules enables edge AI inference workloads up to 350W.

## Key Points

- Supports processors from Intel 6th/7th Gen Desktop (MIC-7700) through Intel Core Ultra Series 2 (MIC-780), plus AMD Ryzen Embedded/EPYC 4005 (MIC-785)
- Modular expansion via i-Module: 1-slot, 2-slot, 4-slot, additional storage, and GPU expansion modules
- GPU i-Module options:
  - MIC-75GF10: up to 80W NVIDIA RTX MXM GPU cards
  - MIC-75M20: up to 80W NVIDIA Data Center / NVIDIA RTX GPU cards
  - MIC-75G20: 1 full-height NVIDIA RTX GPU, up to 350W
  - MIC-75G30: 2 full-height NVIDIA RTX GPUs, up to 350W
- Front-panel Flex I/O supports additional displays, COM ports, DIO, remote switch I/O
- iDoor technology for additional rear-panel I/O expansion
- Target applications: factory and machine automation, machine vision, AMR/MMR robotics, predictive maintenance, smart factories, real-time edge computing
- Software stack: SUSIAccess / SUSI API, WISE-DeviceOn, Ubuntu, Windows 11 IoT LTSC

## Product Line Members

| Model | CPU Generation | Key Differentiator |
|---|---|---|
| [[MIC-7700]] | Intel 6th/7th Gen Desktop LGA1151 | Legacy; DVI output; CFast slot |
| [[MIC-770]] | Intel 8th/9th Gen LGA1151 | H310/Q370 chipset; HDMI; 77mm wide |
| [[MIC-770-V2]] | Intel 10th Gen Xeon/Core LGA1200 | RED; FlexIO/iDoor; -10~50°C |
| [[MIC-770-V3]] | Intel 12th–14th Gen LGA1700 | DDR5; NVMe M.2; IP40; -20~50°C; iBMC 1.2 |
| [[MIC-760]] | Intel 12th–14th Gen LGA1700 | AMR/MMR target; CANbus; 3× GbE; ROS2 |
| [[MIC-780]] | Intel Core Ultra Series 2 LGA1851 | Integrated NPU; DDR5 6400; 3× displays; 195mm wide |
| [[MIC-785]] | AMD Ryzen Embedded / EPYC 4005 AM5 | First AMD option in MIC series |

## Entities Mentioned

[[Advantech]], [[Intel Core Ultra Series 2]], [[Intel 12th-14th Gen Core (Raptor Lake LGA1700)]], [[Intel 10th Gen Xeon W (Comet Lake-S)]], [[Intel 8th-9th Gen Core (LGA1151)]], [[Intel 6th-7th Gen Core Desktop (LGA1151)]], [[AMD Ryzen Embedded AM5]]

## Concepts Introduced or Elaborated

[[i-Module]], [[FlexIO]], [[iDoor]], [[NPU]], [[ROS2]], [[AMR MMR]], [[SUSIAccess]]

## Connections to Existing Wiki

- ARK-3532B and ARK-7060 also support GPU expansion via PCIe x16 slot; MIC-7 i-Module approach adds GPU in compact form without discrete PCIe slot
- ARK-7060 uses IPMI 2.0 (server-grade); MIC-770 V3 and MIC-780 use Advantech iBMC 1.2 (embedded-grade out-of-band management)
- CAN Bus present in ARK-1125H, ARK-3534C/D; MIC-760 adds CAN Bus targeting robotics vs. ARK's IPC/automation focus
- DDR5 in ARK-3534C/D (4800MHz); MIC-770 V3 also DDR5 4800MHz; MIC-780 advances to DDR5 6400MHz

## Open Questions

- GPU i-Module power delivery details (12V auxiliary, smart fan control)
- Full spec tables for MIC-760, MIC-7700, MIC-785 not available in raw data
- i-Module compatibility across MIC generations (MIC-78 series uses its own i-Module variant)
- MIC-75G20 vs MIC-75G30 slot count and TDP limits per slot
