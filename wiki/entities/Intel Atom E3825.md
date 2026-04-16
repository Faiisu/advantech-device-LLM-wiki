---
title: "Intel Atom E3825"
type: entity
tags: [hardware, processor, intel, soc, embedded, bay-trail]
created: 2026-04-16
updated: 2026-04-16
sources: [ARK-1123C, ARK-1123L]
---

# Intel Atom E3825

**Type:** Product (Processor / SoC)  
**Manufacturer:** Intel  
**Family:** Bay Trail-M (Atom E3800 embedded series)  
**Released:** ~2013–2014

## Overview

Dual-core Intel Atom SoC from the Bay Trail-M platform — the embedded-grade variant (E-series) of the Bay Trail generation. Lower-spec than the J1900 quad-core (also Bay Trail but desktop-grade), with half the cores and lower clock speed. Despite this, achieves a wider operating temperature range (-30~70°C) than the J1900-based ARK-1123H (-20~60°C), likely due to lower TDP and thermal design choices.

## Key Specs

- 2 cores, 1.33 GHz (no turbo)
- L2 Cache: 1 MB (vs 2 MB in J1900)
- Memory: DDR3L 1066 MHz (lower speed than J1900's 1333 MHz)
- GPU: Intel Atom SoC integrated; DirectX 11.1, OGL 3.0, OCL 1.1
- TDP: ~6W — lower than J1900's ~10W
- Operating temp (in ARK-1123C/L): **-30~70°C** with extended peripherals

## Comparison vs. Intel Celeron J1900 (Bay Trail-D)

| Spec | E3825 | J1900 |
|---|---|---|
| Cores | 2 | 4 |
| Frequency | 1.33 GHz | 2.0 GHz (burst 2.41) |
| L2 Cache | 1 MB | 2 MB |
| Memory | DDR3L 1066 MHz | DDR3L 1333 MHz |
| TDP | ~6W | ~10W |
| Op. temp (ARK) | -30~70°C | -20~60°C |
| Platform | Bay Trail-M | Bay Trail-D |

## Role in This Wiki

Used in two compact ARK-112X models with different I/O trade-offs:
- [[ARK-1123C]]: dual GbE, 2× RS-232/422/485, no GPIO, Class B EMC
- [[ARK-1123L]]: single GbE, mixed serial, 8-bit GPIO, Class A EMC

## Appearances

[[ARK-1123C]], [[ARK-1123L]]

## Related Entities

[[Advantech]], [[Intel Celeron J1900]]

## Related Concepts

[[Fanless Embedded PC]], [[Industrial IO]]
