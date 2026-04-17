---
title: "Intel 10th Gen Xeon W (Comet Lake-S)"
type: entity
tags: [processor, intel, comet-lake, embedded, xeon, lga1200, ecc]
created: 2026-04-16
updated: 2026-04-17
sources: [ARK-3532B, ARK-3532C, MIC-770-V2]
---

# Intel 10th Gen Xeon W (Comet Lake-S)

**Type:** Processor Platform  
**Also known as:** Comet Lake-S Embedded, LGA1200 Embedded, 10th Gen Core embedded

## Overview

Intel's 10th Generation Core and Xeon W processors in the LGA1200 socketed form factor, embedded variants (E/TE suffix). Manufactured on 14nm. The embedded series (W480E chipset) adds ECC DDR4 support across all tiers from Celeron to Xeon W. Up to 10 cores (Xeon W-1290TE). Used in the ARK-3532 sub-series — the first LGA-socketed platform in this wiki (all prior ARK models use BGA or soldered SoCs).

## Key Facts

| SKU | Cores | TDP | Notes |
|---|---|---|---|
| Xeon W-1290TE | 10 | 35W (T = low-power) | Workstation-grade; highest in class |
| Core i9-10900E | 10 | 65W | High-end desktop |
| Core i7-10700E | 8 | 65W | — |
| Core i5-10500E | 6 | 65W | — |
| Core i3-10100E | 4 | 65W | — |
| Celeron G5900E | 2 | 65W | Entry-level |

- **Chipset:** Intel W480E (embedded variant of W480)
- **Socket:** LGA1200 (socketed — CPU can be upgraded or swapped)
- **Memory:** DDR4 2933MHz, up to 64 GB (2× SO-DIMM); ECC supported on Xeon W and higher Core i variants
- **Graphics:** Intel UHD Graphics 630; DirectX 12, OpenGL 4.4; H.265/HEVC encode/decode
- **PCIe:** Gen 3; supports PCIe x16 for discrete GPU (via ARK-3532B)

## Role in This Wiki

Powers three products: [[ARK-3532B]] and [[ARK-3532C]] (expansion box PCs using W480E with ECC) and [[MIC-770-V2]] (compact box PC using H420E/W480E chipset, no ECC confirmed). The W480E chipset bridges industrial reliability (ECC, long lifecycle) with workstation-class performance in the ARK-3532 line; MIC-770 V2 uses the same CPU generation but in a compact 77mm form factor without the PCIe expansion slots.

## Appearances

[[ARK-3532B]], [[ARK-3532C]], [[MIC-770-V2]]

## Related Entities

[[Advantech]], [[Intel 6th Gen Core (Skylake-H)]], [[Intel 12th-14th Gen Core (Raptor Lake LGA1700)]]

## Related Concepts

[[Fanless Embedded PC]], [[Industrial IO]], [[DeviceOn]]
