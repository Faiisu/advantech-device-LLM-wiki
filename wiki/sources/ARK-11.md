---
title: "ARK-11"
type: source
tags: [hardware, embedded, industrial-pc, fanless, advantech, din-rail, n3350]
created: 2026-04-16
updated: 2026-04-16
sources: [self]
---

# ARK-11

**Type:** Product Specification Sheet  
**Author(s):** Advantech  
**Origin:** `raw/ARK-11.md` | https://www.advantech.com/th-th/products/1-2jkbyz/ark-11/

## Summary

DIN-rail fanless box PC on Intel Celeron N3350 (Apollo Lake, dual-core). Notable for -30–70°C extended temperature range (widest in the series), built-in 8 GB RAM and 128 GB SSD, Windows 10 IoT Enterprise pre-installed, Advantech WISE-PaaS/DeviceOn support, and 12–28V wide-range power input. I/O ports are front-facing bezel (DIN-rail style).

## Key Specs

- **CPU:** Intel Celeron N3350, 2-core, 1.1 GHz (burst 2.4 GHz); Apollo Lake
- **Memory:** DDR3L 1600 MHz, up to 8 GB, 2× SO-DIMM; **8 GB built-in**
- **Display:** 2× HDMI (4K)
- **GPU:** Intel HD Graphics 500 (Gen9); DirectX 12, OpenCL 2.0, H.265/HEVC
- **Ethernet:** 2× Intel i210 GbE (Wake on LAN)
- **Serial:** 2× RS-232/422/485 with auto flow control; COM2 with 5V/12V power supply
- **USB:** 4× USB 3.0
- **GPIO:** 8-bit (optional)
- **Storage:** 1× 128 GB TLC SSD (-40–85°C rated) built-in; 1× full-size mSATA (shares mPCIe slot)
- **Expansion:** 1× full-size mPCIe with SIM holder; 1× M.2 2230 E key (WiFi)
- **Power:** 12–28 VDC wide range; 60W adapter included; typical **6.4W**, max 18.1W
- **Operating temp:** -30–70°C (with extended peripherals); 0–40°C with HDD
- **Dimensions:** 53.5 × 158 × 114 mm; 1.2 kg
- **Mounting:** DIN-rail / Wall
- **OS:** Windows 10 IoT Enterprise (built-in); Linux by project
- **Certifications:** CE/FCC Class B, CCC, BSMI; UL/CB 62368

## Differentiators vs. ARK Series

- **Widest operating temperature** in the sub-series: -30–70°C
- Only model with WISE-PaaS/DeviceOn (Advantech cloud IoT platform) pre-configured
- Windows 10 IoT Enterprise built-in — OEM-ready
- 12–28V wide range input — suits vehicle/industrial power rail variation
- Front-facing I/O on DIN-rail bezel — designed for panel/rail integration

## Entities Mentioned

[[Advantech]], [[Intel Celeron N3350]]

## Concepts Introduced or Elaborated

[[Fanless Embedded PC]], [[DIN-Rail Mounting]], [[Industrial IO]], [[DeviceOn]]

## Connections to Existing Wiki

- Same J-series/N-series Apollo Lake lineage — compare [[Intel Celeron J1900]] (Bay Trail predecessor)
- DIN-rail form factor first introduced in this series
- Wide-range power (12–28V) contrasts with fixed 12V in [[ARK-6322]] and [[ARK-10]]

## Open Questions

- WISE-PaaS vs DeviceOn — are these the same platform or different generations?
- What does the optional 8-bit GPIO connect to in a typical deployment?
