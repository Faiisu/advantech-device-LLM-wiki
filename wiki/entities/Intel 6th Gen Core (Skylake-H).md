---
title: "Intel 6th Gen Core (Skylake-H)"
type: entity
tags: [processor, intel, skylake, embedded, bga]
created: 2026-04-16
updated: 2026-04-16
sources: [ARK-3520L]
---

# Intel 6th Gen Core (Skylake-H)

**Type:** Processor Platform  
**Also known as:** Skylake-H, 6th Generation Intel Core (H-series)

## Overview

Intel's 6th Generation Core processor family in the H-series (high-performance mobile), manufactured on 14nm. The embedded BGA variants (i5-6440EQ, i7-6820EQ) are designed for soldered-down deployment in fanless industrial computers. QM170 chipset provides PCIe lanes for discrete GPU support. Introduced in 2015.

## Key Facts

| SKU | Cores | Base Freq | TDP | L3 Cache | Used In |
|---|---|---|---|---|---|
| Core i5-6440EQ | 4 | 2.7 GHz | 45W | 6 MB | ARK-3520L (U7A1E SKU) |
| Core i7-6820EQ | 4 | 2.8 GHz | 45W | 8 MB | ARK-3520L (U8A1E SKU) |

- **Chipset:** Intel QM170
- **Memory:** DDR4 2133MHz, up to 32 GB (SO-DIMM), no ECC
- **Graphics:** Intel HD Graphics Gen 9; DirectX 12, OpenGL 4.4; hardware H.265/HEVC encode/decode
- **Form factor:** BGA (soldered) — not socketed; CPU is fixed at purchase
- **Process node:** 14nm (first 14nm generation from Intel)

## Role in This Wiki

The Skylake-H BGA platform is used in the [[ARK-3520L]], the oldest ARK-3000 series model ingested. Represents the entry point of the "Expansion Box PC" tier — higher TDP (45W) than any ARK-1000/1200 processor, enabling triple-display, 8× COM, and an AMO-3xxx riser card for PCI/PCIe expansion.

## Appearances

[[ARK-3520L]]

## Related Entities

[[Advantech]], [[Intel Celeron J1900]], [[Intel 10th Gen Xeon W (Comet Lake-S)]]

## Related Concepts

[[Fanless Embedded PC]], [[Mini PCIe]], [[iDoor]]
