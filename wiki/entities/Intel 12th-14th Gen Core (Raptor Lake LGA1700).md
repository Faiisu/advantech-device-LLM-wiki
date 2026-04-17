---
title: "Intel 12th-14th Gen Core (Raptor Lake LGA1700)"
type: entity
tags: [processor, intel, alder-lake, raptor-lake, embedded, lga1700, ddr5, ecc]
created: 2026-04-16
updated: 2026-04-17
sources: [ARK-3534C, ARK-3534D, MIC-760, MIC-770-V3]
---

# Intel 12th-14th Gen Core (Raptor Lake LGA1700)

**Type:** Processor Platform  
**Also known as:** Alder Lake / Raptor Lake / Raptor Lake Refresh (LGA1700 embedded), 12th/13th/14th Gen Core embedded

## Overview

Intel's 12th through 14th Generation Core processors in the LGA1700 socketed form factor, 65W embedded series. Manufactured on Intel 7 process node (10nm ESF). The same silicon family spans Alder Lake (12th Gen, 2021), Raptor Lake (13th Gen, 2022), and Raptor Lake Refresh (14th Gen, 2023) — all socket-compatible on LGA1700. Introduces DDR5 memory, significant IPC improvements over 10th Gen, and (with R680E chipset) ECC support. Used in the ARK-3534 sub-series.

## Key Facts

- **Generations:** 12th (Alder Lake), 13th (Raptor Lake), 14th (Raptor Lake Refresh) — same LGA1700 socket
- **TDP class in ARK-3534:** 65W embedded series
- **Chipsets used:**
  - **H610E** — used in ARK-3534C; no ECC support
  - **R680E** — used in ARK-3534D; ECC DDR5 support
- **Memory:** DDR5 4800MHz, up to 64 GB (2× SO-DIMM); ECC on R680E only
- **PCIe:** Gen 4 capable; PCIe x16 slot + PCIe x4 (on R680E) or PCIe x16 only (H610E)
- **Note on naming:** Advantech spec sheets refer to "Intel 12/13/14th Gen 65W Embedded Series" — specific SKUs not listed

## Chipset Comparison (in ARK-3534 context)

| Chipset | ECC | PCIe x4 slot | GbE ports | RAID | Used In |
|---|---|---|---|---|---|
| H610E | No | No | 2× | No | ARK-3534C |
| R680E | Yes | Yes | 4× | SW RAID | ARK-3534D |

## Chipset Comparison Across Wiki Models

| Chipset | ECC | RAID | DDR5 | Used In |
|---|---|---|---|---|
| H610E | No | No | 4800MHz | ARK-3534C, MIC-770 V3 (H610E narrow variant) |
| R680E | Yes | SW RAID | 4800MHz | ARK-3534D, MIC-770 V3 (R680E wide variant) |
| R680E (MIC) | No (MIC-770 V3) | SW RAID | 4800MHz | MIC-770 V3 — note: R680E used but ECC not confirmed for MIC variant |

## Role in This Wiki

Powers four products across two product lines: [[ARK-3534C]], [[ARK-3534D]] (expansion box PCs) and [[MIC-760]], [[MIC-770-V3]] (compact box PCs). Same CPU generation as the ARK-1125 series (Alder Lake-N) but at desktop-class 65W TDP. The MIC-770 V3 adds IP40 dust protection, iBMC 1.2, and NVMe M.2 vs the ARK-3534 expansion box approach.

## Appearances

[[ARK-3534C]], [[ARK-3534D]], [[MIC-760]], [[MIC-770-V3]]

## Related Entities

[[Advantech]], [[Intel 10th Gen Xeon W (Comet Lake-S)]], [[Intel Atom x7211E]], [[Intel N200]]

## Related Concepts

[[Fanless Embedded PC]], [[CAN Bus]], [[IEC 62443]], [[DeviceOn]]
