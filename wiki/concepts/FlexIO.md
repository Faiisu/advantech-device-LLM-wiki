---
title: "FlexIO"
type: concept
tags: [advantech, flexio, flex-io, expansion, front-panel, io]
created: 2026-04-17
updated: 2026-04-17
sources: [MIC-770-V2, MIC-770-V3, MIC-785, mic-7000-series-overview]
---

# FlexIO

## Definition

Flex I/O (FlexIO) is Advantech's front-panel modular I/O expansion kit for MIC-series compact box PCs. Located on the front panel for convenient cabling, FlexIO slots accept interchangeable modules that add display outputs, COM ports, DIO channels, or remote switch I/O without modifying the base unit's rear panel.

## Why It Matters

FlexIO addresses the scenario where the standard fixed I/O of a compact box PC is insufficient for a given application, but a full i-Module (PCIe expansion) is unnecessary. It allows quick, front-accessible reconfiguration — useful in machine automation where cabling runs are front-facing.

## Key Properties

- Located on the front panel (vs iDoor which is rear-panel)
- Supported expansion types include: additional HDMI, DVI, DisplayPort, COM ports, DIO, remote switch I/O
- Available as Advantech Flex I/O Expansion Kit (separate purchasable product family)
- Introduced in MIC-770 V2; absent in MIC-770 V1 and MIC-7700
- Works alongside, not instead of, i-Module (i-Module provides PCIe slots; FlexIO provides port modules)

## Evidence and Examples

- [[MIC-770-V2]]: "Supports Advantech i-Modules, FlexIO and iDoor technology, flexible configure additional HDMI, DVI, Comport, DIO, Remote switch IO"
- [[MIC-770-V3]]: "Supports FlexIO and iDoor technology, flexible configure additional DP, DVI, COM port, DIO, Remote switch IO"
- [[MIC-785]]: "Supports FlexIO, iDoor and iModule technology"

## Tensions and Contradictions

- FlexIO and iDoor serve overlapping purposes (both add I/O); the distinction is front-panel (FlexIO) vs rear-panel/secondary-chassis (iDoor). In practice, a system can use both simultaneously.
- Not all MIC models support FlexIO: MIC-770 V1, MIC-7700, and MIC-760 are not listed as FlexIO-compatible in raw data.

## Related Concepts

[[iDoor]], [[i-Module]], [[Industrial IO]], [[Fanless Embedded PC]]

## Sources

[[MIC-770-V2]], [[MIC-770-V3]], [[MIC-785]], [[mic-7000-series-overview]]
