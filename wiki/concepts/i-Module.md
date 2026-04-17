---
title: "i-Module"
type: concept
tags: [advantech, expansion, pcie, modular, gpu, i-module]
created: 2026-04-17
updated: 2026-04-17
sources: [mic-7000-series-overview, MIC-770, MIC-770-V2, MIC-770-V3, MIC-7700, MIC-780, MIC-785]
---

# i-Module

## Definition

i-Module is Advantech's proprietary modular expansion chassis system for MIC-series compact box PCs. An i-Module attaches to the host system to add PCIe slots, storage bays, or GPU capability without changing the base unit. The host system provides PCIe lanes and 12VDC power to the i-Module via an internal connector.

## Why It Matters

i-Module enables a single base platform (e.g., MIC-770 V3) to be configured for different application requirements — from basic I/O expansion to full-height dual-GPU edge AI inference — without redesigning the system or the application software. This reduces CTOS (Configure-To-Order System) lead time.

## Key Properties

- Slot variants: 1-slot, 2-slot, 4-slot PCIe expansion; dedicated storage; GPU expansion
- GPU-specific i-Module options (MIC-7 series):
  - **MIC-75GF10**: supports up to 80W NVIDIA RTX MXM GPU cards (compact form)
  - **MIC-75M20**: supports up to 80W NVIDIA Data Center / NVIDIA RTX GPU cards
  - **MIC-75G20**: 1× full-height NVIDIA RTX GPU, up to 350W
  - **MIC-75G30**: 2× full-height NVIDIA RTX GPU, up to 350W
- MIC-78 series (MIC-780, MIC-785) uses its own i-Module variant — not cross-compatible with MIC-770 i-Modules
- Optional smart system fans and 12VDC auxiliary power for thermal management in GPU i-Modules
- iDoor is a related but distinct Advantech I/O expansion mechanism targeting additional port modules (not PCIe card slots)

## Evidence and Examples

- [[MIC-770]] (V1/V2/V3) all support i-Module for PCIe expansion
- [[MIC-780]] uses "MIC-78 series i-Module" — separate product family
- [[MIC-785]] supports i-Module, FlexIO, and iDoor
- [[MIC-7700]] supports i-Module (legacy, first generation)

## Tensions and Contradictions

- MIC-78 series i-Module incompatibility with MIC-770 i-Modules creates an upgrade barrier — customers cannot reuse existing i-Modules when switching from MIC-770 to MIC-780.
- ARK-3000 series (expansion box PCs) provide a similar function to i-Modules but in a different physical form — ARK-3000 is a larger standalone chassis, i-Module attaches directly to the base unit.

## Related Concepts

[[FlexIO]], [[iDoor]], [[Fanless Embedded PC]], [[Mini PCIe]]

## Sources

[[mic-7000-series-overview]], [[MIC-770]], [[MIC-770-V2]], [[MIC-770-V3]], [[MIC-7700]], [[MIC-780]], [[MIC-785]]
