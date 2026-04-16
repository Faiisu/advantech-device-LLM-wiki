---
title: "Wiki Index"
updated: 2026-04-16
---

# Wiki Index

> Master catalog of all pages in this wiki. Updated by the wiki-agent on every ingest, query (if filed), and lint pass. Read this first when answering queries.

---

## Sources (`wiki/sources/`)

### Advantech ARK Hardware

#### ARK-6000 Series

| Page | CPU | Key Trait |
|---|---|---|
| [[ARK-6322]] | J1900 | 6× COM, 8× USB, 200×64mm box, 15.7W |

#### ARK-1000 / 1100 Series

| Page | CPU | Key Trait |
|---|---|---|
| [[ARK-10]] | J1900 | Built-in 2GB RAM + 500GB HDD, VGA only |
| [[ARK-11]] | N3350 | DIN-rail, -30–70°C, DeviceOn, 12–28V, 6.4W |
| [[ARK-1123H]] | J1900 | Compact box, dual HDMI, SUSIAccess, RED option |
| [[ARK-1123C]] | E3825 | Compact box, dual GbE, -30–70°C, FCC Class B |
| [[ARK-1123L]] | E3825 | Compact box, single GbE, 8-bit GPIO, FCC Class A, -30–70°C |
| [[ARK-1124C]] | N3350 | DIN-rail, 4× COM, single GbE, iDoor |
| [[ARK-1124H]] | E3940 | DIN-rail, dual HDMI 4K, TPM 2.0, iDoor |
| [[ARK-1125C]] | x7211E | DIN-rail, DDR5, 4× COM, IEC 62443-4-2 SL2 |
| [[ARK-1125H]] | N200 | DIN-rail, DDR5, 2× CAN Bus, dual 2.5GbE, RED |

#### ARK-1200 Series

| Page | CPU | Key Trait |
|---|---|---|
| [[ARK-1220F]] | E3940 | DIN-rail, 2.5 kV isolated GbE + COM + GPIO |
| [[ARK-1220L]] | E3940 | DIN-rail, dual HDMI 4K, -30–70°C, WISE-PaaS |
| [[ARK-1221L]] | x6413E | DIN-rail, DDR4 32GB, -40°C, HDMI+DP, 1× CAN |

#### ARK-1500 Series

| Page | CPU | Key Trait |
|---|---|---|
| [[ARK-1250L]] | Core i5-11th | DIN-rail, 64GB DDR4, triple GbE, 4× COM, -40°C |
| [[ARK-1551]] | Core i5-8th | Slim wall-mount, swappable bay, RAID, NVMe, RED |

#### ARK-3000 Series (Expansion Box PCs)

| Page | CPU | Key Trait |
|---|---|---|
| [[ARK-3520L]] | Core i5/i7-6th BGA | 8× COM, triple display, iDoor, AMO-3xxx riser |
| [[ARK-3532B]] | Xeon W / Core i-10th | PCIe x16 GPU slot, ECC DDR4, TPM 2.0, 4× GbE |
| [[ARK-3532C]] | Xeon W / Core i-10th | 2× PCI legacy, ECC DDR4, 4× GbE |
| [[ARK-3534C]] | Core i-12/13/14th | DDR5, 2× CAN Bus, IEC 62443-4-2 SL2, 2× GbE |
| [[ARK-3534D]] | Core i-12/13/14th | DDR5 ECC, 2× CAN Bus, IEC 62443-4-2 SL2, 4× GbE |

#### ARK-7000 Series (Extreme Performance Box PCs)

| Page | CPU | Key Trait |
|---|---|---|
| [[ARK-7060]] | Xeon D-1746TER / D-1715TER | **Fan-cooled, AC power, IPMI 2.0**, 128GB ECC DDR4, opt 10GbE |

---

## Entities (`wiki/entities/`)

### Organisations

- [[Advantech]] — Industrial PC manufacturer; ARK-6000/1000/1200/1500/3000/7000 product lines.

### Processors — Bay Trail (2013–2014)

| Page | Cores | TDP | Used In |
|---|---|---|---|
| [[Intel Celeron J1900]] | 4 | ~10W | ARK-6322, ARK-10, ARK-1123H |
| [[Intel Atom E3825]] | 2 | ~6W | ARK-1123C, ARK-1123L |

### Processors — Apollo Lake (2016–2017)

| Page | Cores | TDP | Used In |
|---|---|---|---|
| [[Intel Celeron N3350]] | 2 | ~6W | ARK-11, ARK-1124C |
| [[Intel Atom E3940]] | 4 | ~9.5W | ARK-1124H, ARK-1220F, ARK-1220L |

### Processors — Whiskey / Elkhart / Tiger Lake (2018–2021)

| Page | Platform | Used In |
|---|---|---|
| [[Intel Core i5-8365UE]] | Whiskey Lake | ARK-1551 |
| [[Intel Atom x6413E]] | Elkhart Lake | ARK-1221L |
| [[Intel Core i5-1145G7E]] | Tiger Lake | ARK-1250L |

### Processors — Alder Lake-N (2023)

| Page | Used In |
|---|---|
| [[Intel Atom x7211E]] | ARK-1125C |
| [[Intel N200]] | ARK-1125H |

### Processors — ARK-3000 Expansion Tier

| Page | Platform | TDP | Used In |
|---|---|---|---|
| [[Intel 6th Gen Core (Skylake-H)]] | Skylake-H BGA | 45W | ARK-3520L |
| [[Intel 10th Gen Xeon W (Comet Lake-S)]] | Comet Lake LGA1200 | 35–65W | ARK-3532B, ARK-3532C |
| [[Intel 12th-14th Gen Core (Raptor Lake LGA1700)]] | Raptor Lake LGA1700 | 65W | ARK-3534C, ARK-3534D |

### Processors — ARK-7000 Extreme Performance Tier

| Page | Platform | TDP | Used In |
|---|---|---|---|
| [[Intel Xeon D-1700 (Ice Lake-D)]] | Ice Lake-D SoC | 50–67W | ARK-7060 |

---

## Concepts (`wiki/concepts/`)

### Hardware & Form Factor

- [[Fanless Embedded PC]] — Passive-cooled industrial PC; no moving parts; spans compact DIN-rail to large expansion box tiers. ARK-7060 is fan-cooled (not covered by this concept).
- [[DIN-Rail Mounting]] — 35mm industrial rail standard; dominant in control panel integration.
- [[Mini PCIe]] — Compact PCIe expansion slot for WLAN, WWAN, mSATA in embedded platforms.
- [[iDoor]] — Advantech modular I/O expansion system; optional second-layer chassis add-on.

### Industrial IO & Connectivity

- [[Industrial IO]] — Serial/digital interfaces for field devices: RS-232/422/485, GPIO, GbE.
- [[CAN Bus]] — Automotive/industrial differential serial bus; 2-wire, multi-master. Models: ARK-1125H (2×), ARK-1221L (1×), ARK-1250L (opt), ARK-3534C/D (2×).
- [[Isolated IO]] — Galvanic isolation on I/O ports; protects against ground faults. Only model: ARK-1220F (2.5 kV).
- [[IPMI]] — Server-grade out-of-band management (hardware-level, OS-independent). Only model: ARK-7060 (IPMI 2.0, Aspeed AST2500 BMC).

### Software & Platform

- [[DeviceOn]] — Advantech IoT device management platform; OTA updates, monitoring, AI deployment.
- [[SUSIAccess]] — Advantech embedded software API for hardware feature access; older generation.
- [[IEC 62443]] — OT cybersecurity standard; SL2 certified models: ARK-1125C, ARK-3534C, ARK-3534D.

---

## Synthesis (`wiki/synthesis/`)

- [[advantech-ark-series-comparison]] — Master comparison table: all 21 ARK models, CPU, COM, CAN, temp, RAM, RED, form factor.
- [[ARK-1123x]] — Sub-series hub: ARK-1123H vs ARK-1123C vs ARK-1123L. Axis: HDMI / temp / GPIO / EMC class.
- [[ARK-1124x]] — Sub-series hub: ARK-1124C vs ARK-1124H. Axis: COM count vs HDMI + TPM 2.0.
- [[ARK-1125x]] — Sub-series hub: ARK-1125C vs ARK-1125H. Axis: IEC 62443 vs CAN Bus + RED.
- [[ARK-3532x]] — Sub-series hub: ARK-3532B vs ARK-3532C. Axis: PCIe x16 GPU vs PCI legacy.
- [[ARK-3534x]] — Sub-series hub: ARK-3534C vs ARK-3534D. Axis: H610E (no ECC) vs R680E (ECC, 4× GbE).

---

**Total pages:** 52 | **Last updated:** 2026-04-16
