---
title: "Wiki Index"
updated: 2026-04-17
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

### Advantech MIC Hardware

#### MIC-7 Series Overview

- [[mic-7000-series-overview]] — Family overview: MIC-7700→MIC-785, i-Module GPU options, target applications

#### MIC-770x Sub-Series (Compact 77mm Box PCs, generational)

| Page | CPU | Key Trait |
|---|---|---|
| [[MIC-7700]] | Intel 6th/7th Gen LGA1151 | Legacy; DVI; CFast; SIM; 9–36V |
| [[MIC-770]] | Intel 8th/9th Gen LGA1151 | HDMI; H310/Q370; 64GB DDR4; -10~40°C |
| [[MIC-770-V2]] | Intel 10th Gen Xeon/Core LGA1200 | RED; FlexIO; iDoor; -10~50°C |
| [[MIC-770-V3]] | Intel 12th–14th Gen LGA1700 | DDR5 128GB; NVMe M.2; IP40; iBMC 1.2; -20~50°C |

**Hub:** [[MIC-770x]] — generational comparison and selection guide

#### MIC-760 (AMR/MMR Controller)

| Page | CPU | Key Trait |
|---|---|---|
| [[MIC-760]] | Intel 12th–14th Gen LGA1700 | AMR/MMR; CANbus; 3× GbE; WiFi 36ms; ROS2; Ubuntu |

#### MIC-78x Sub-Series (Compact 195mm Box PCs, latest gen)

| Page | CPU | Key Trait |
|---|---|---|
| [[MIC-780]] | Intel Core Ultra 5/7/9 Series 2 LGA1851 | **Integrated NPU**; DDR5 6400MHz; 3× display; DIN rail |
| [[MIC-785]] | AMD Ryzen Embedded / EPYC 4005 AM5 | **First AMD**; machine vision; iBMC 1.2 |

**Hub:** [[MIC-78x]] — Intel Core Ultra vs AMD comparison

---

## Entities (`wiki/entities/`)

### Organisations

- [[Advantech]] — Industrial PC manufacturer; ARK-series and MIC-7 series product lines.

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

### Processors — Desktop Socketed (MIC-7700 through MIC-770 V2)

| Page | Platform | TDP | Used In |
|---|---|---|---|
| [[Intel 6th-7th Gen Core Desktop (LGA1151)]] | Skylake/Kaby Lake LGA1151 v1 | 65W | MIC-7700 |
| [[Intel 8th-9th Gen Core (LGA1151)]] | Coffee Lake LGA1151 v2 | 65W | MIC-770 |
| [[Intel 6th Gen Core (Skylake-H)]] | Skylake-H BGA | 45W | ARK-3520L |
| [[Intel 10th Gen Xeon W (Comet Lake-S)]] | Comet Lake LGA1200 | 35–65W | ARK-3532B, ARK-3532C, MIC-770 V2 |
| [[Intel 12th-14th Gen Core (Raptor Lake LGA1700)]] | Raptor Lake LGA1700 | 65W | ARK-3534C, ARK-3534D, MIC-760, MIC-770 V3 |

### Processors — Latest Generation (MIC-78x)

| Page | Platform | TDP | Used In |
|---|---|---|---|
| [[Intel Core Ultra Series 2]] | Meteor Lake LGA1851 | 65W | MIC-780 |
| [[AMD Ryzen Embedded AM5]] | Zen 4 AM5 (LGA1718) | varies | MIC-785 |

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
- [[iDoor]] — Advantech rear-panel modular I/O expansion; ARK-6322, ARK-1124x, MIC-770 V2/V3, MIC-785.
- [[i-Module]] — Advantech modular PCIe/GPU expansion chassis; attaches to MIC-7 series; GPU options up to 350W.
- [[FlexIO]] — Advantech front-panel I/O expansion kit; adds display/COM/DIO modules; MIC-770 V2/V3, MIC-785.
- [[NPU]] — Neural Processing Unit; integrated AI accelerator in Intel Core Ultra; MIC-780 is first fanless IPC with NPU.

### Industrial IO & Connectivity

- [[Industrial IO]] — Serial/digital interfaces for field devices: RS-232/422/485, GPIO, GbE.
- [[CAN Bus]] — Automotive/industrial differential serial bus; 2-wire, multi-master. Models: ARK-1125H (2×), ARK-1221L (1×), ARK-1250L (opt), ARK-3534C/D (2×), MIC-760 (CANbus, count unspec.).
- [[Isolated IO]] — Galvanic isolation on I/O ports; protects against ground faults. Only ARK model: ARK-1220F (2.5 kV).
- [[IPMI]] — Server-grade out-of-band management (hardware-level, OS-independent). Only model: ARK-7060 (IPMI 2.0, Aspeed AST2500 BMC).
- [[EtherCAT]] — Real-time Industrial Ethernet fieldbus; deterministic motion control; MIC-760 ROS2 node support.

### Robotics & AI

- [[AMR MMR]] — Autonomous Mobile Robot / Material Movement Robot; compute requirements; MIC-760 target platform.
- [[ROS2]] — Robot Operating System 2; open robotics middleware; MIC-760 ships with ROS2 (EtherCAT + Modbus nodes).

### Software & Platform

- [[DeviceOn]] — Advantech IoT device management platform; OTA updates, monitoring, AI deployment.
- [[SUSIAccess]] — Advantech embedded software API (also called SUSI API); hardware feature access across ARK and MIC series.
- [[IEC 62443]] — OT cybersecurity standard; SL2 certified models: ARK-1125C, ARK-3534C, ARK-3534D.

---

## Synthesis (`wiki/synthesis/`)

- [[advantech-ark-series-comparison]] — Master comparison table: all 21 ARK models, CPU, COM, CAN, temp, RAM, RED, form factor.
- [[ARK-1123x]] — Sub-series hub: ARK-1123H vs ARK-1123C vs ARK-1123L. Axis: HDMI / temp / GPIO / EMC class.
- [[ARK-1124x]] — Sub-series hub: ARK-1124C vs ARK-1124H. Axis: COM count vs HDMI + TPM 2.0.
- [[ARK-1125x]] — Sub-series hub: ARK-1125C vs ARK-1125H. Axis: IEC 62443 vs CAN Bus + RED.
- [[ARK-3532x]] — Sub-series hub: ARK-3532B vs ARK-3532C. Axis: PCIe x16 GPU vs PCI legacy.
- [[ARK-3534x]] — Sub-series hub: ARK-3534C vs ARK-3534D. Axis: H610E (no ECC) vs R680E (ECC, 4× GbE).
- [[MIC-770x]] — Sub-series hub: MIC-7700 → MIC-770 → V2 → V3. Generational comparison + selection guide.
- [[MIC-78x]] — Sub-series hub: MIC-780 (Intel Core Ultra + NPU) vs MIC-785 (AMD AM5).
- [[mic-series-comparison]] — Master comparison table: all 8 MIC-7 models, CPU, memory, temp, features, application guide.

---

**Total pages:** 73 | **Last updated:** 2026-04-17
