---
title: "Intel Xeon D-1700 (Ice Lake-D)"
type: entity
tags: [processor, intel, xeon, ice-lake-d, embedded, ecc, server-grade]
created: 2026-04-16
updated: 2026-04-16
sources: [ARK-7060]
---

# Intel Xeon D-1700 (Ice Lake-D)

**Type:** Processor  
**Manufacturer:** Intel  
**Platform:** Ice Lake-D (SoC — on-package memory controller + SoC architecture)  
**Generation:** 2nd Gen Xeon D (Ice Lake)

## Overview

The Intel Xeon D-1700 series is an embedded server-class SoC designed for edge computing, NAS, networking, and industrial automation workloads requiring high core count and ECC memory in a compact power envelope. Unlike desktop-class LGA processors (used in ARK-3532/3534), the Xeon D is a BGA SoC with integrated memory controller and networking features. The "T" suffix in model names (e.g., D-1746TER) indicates extended temperature range; "E" suffix indicates embedded lifecycle support; "R" indicates TSN/enhanced networking.

## Key Facts

- **SKUs in this wiki:** D-1746TER (10 cores, 15MB L3, 67W TDP) and D-1715TER (4 cores, 10MB L3, 50W TDP)
- **Memory:** DDR4 2933MHz; up to 128GB ECC via 4× SO-DIMM (in ARK-7060 implementation)
- **ECC:** Yes — native ECC support
- **Management:** Supports IPMI 2.0 via Aspeed AST2500 BMC integration
- **Networking:** Supports optional 10GbE (Intel X550) via AMO module
- **Temperature range:** Extended temp variants (TER suffix) — -10~50°C operating in ARK-7060 with airflow

## Role in This Wiki

Used exclusively in [[ARK-7060]]. Represents the highest-performance and highest-TDP platform ingested in this wiki. First server-grade SoC processor (Xeon class) among the ARK sources; contrasts with desktop-class Xeon W used in [[ARK-3532B]] and [[ARK-3532C]].

## Appearances

[[ARK-7060]]

## Related Entities

[[Advantech]], [[Intel 10th Gen Xeon W (Comet Lake-S)]]

## Related Concepts

[[IPMI]], [[Fanless Embedded PC]]
