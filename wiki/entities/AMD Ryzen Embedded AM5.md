---
title: "AMD Ryzen Embedded AM5"
type: entity
tags: [amd, processor, am5, ryzen-embedded, epyc, zen4, lga1718]
created: 2026-04-17
updated: 2026-04-17
sources: [MIC-785, mic-7000-series-overview]
---

# AMD Ryzen Embedded AM5

**Type:** Processor
**Also known as:** AMD Ryzen Embedded 7000/9000 series; AMD EPYC 4005 series; AM5 socket (LGA1718); Zen 4 / Zen 4c architecture

## Overview

AMD Ryzen Embedded 7000/9000 and EPYC 4005 processors use the AM5 platform (LGA1718 socket) based on Zen 4 / Zen 4c microarchitecture. The AM5 platform supports DDR5 memory and PCIe Gen5. AMD EPYC 4005 targets server-class workloads at the embedded edge (more cores, ECC support); Ryzen Embedded 7000/9000 targets high-performance desktop-class workloads with integrated Radeon graphics for machine vision.

## Key Facts

- Socket: AM5 (LGA1718)
- Architecture: Zen 4 / Zen 4c
- Memory: DDR5 (speed and capacity vary by SKU)
- Graphics: integrated Radeon RDNA 3 (varies by SKU)
- EPYC 4005: server-lineage, more cores, ECC DDR5 capable
- Ryzen Embedded 7000/9000: consumer/prosumer lineage, strong integrated GPU, no ECC on base SKUs
- PCIe Gen5 support (AM5 platform)

## Role in This Wiki

The AMD Ryzen Embedded AM5 platform powers the [[MIC-785]], making it the sole AMD-based product in this entire wiki. It is positioned for machine vision and high-end machine controller applications where AMD's integrated GPU or EPYC's multi-core density provides an advantage over Intel alternatives in the same price band.

## Appearances

[[MIC-785]], [[mic-7000-series-overview]]

## Related Entities

[[Advantech]], [[Intel Core Ultra Series 2]]

## Related Concepts

[[Fanless Embedded PC]], [[i-Module]], [[FlexIO]], [[iDoor]]

## Tensions and Contradictions

- EPYC 4005 and Ryzen Embedded 7000/9000 are very different market segments (server vs desktop embedded); Advantech supporting both on one board suggests broad CPU flexibility, but the raw data does not clarify which SKU is primary or whether ECC is validated.
