---
updated: 2026-04-17
session: 6
---

# Hotcache

> Rolling summary of recent wiki activity (~500 words max). Read this before index.md or any wiki file. If the answer is here, skip further reads. Overwrite entirely each update — do not append.

---

## Wiki Domain

This wiki covers **Advantech industrial and edge PCs** — two product families:
- **ARK series**: fanless box PCs, DIN-rail computers, expansion box PCs, server-grade extreme performance PCs (21 models)
- **MIC-7 series**: compact modular box PCs with i-Module expansion (8 models, added 2026-04-17)

---

## MIC-7 Series — Just Ingested (8 models)

| Model | CPU | Socket | Key Trait |
|---|---|---|---|
| MIC-7700 | Intel 6th/7th Gen | LGA1151 v1 | Legacy; DVI (not HDMI); CFast; SIM slot; 9–36V |
| MIC-770 | Intel 8th/9th Gen | LGA1151 v2 | HDMI; H310/Q370; DDR4 64GB; -10~40°C; 77mm |
| MIC-770 V2 | Intel 10th Gen Xeon/Core | LGA1200 | RED; FlexIO; iDoor; -10~50°C; Azure/AWS certs |
| MIC-770 V3 | Intel 12th–14th Gen | LGA1700 | DDR5 128GB; NVMe M.2; IP40; iBMC 1.2; -20~50°C |
| MIC-760 | Intel 12th–14th Gen | LGA1700 | AMR/MMR; CANbus; 3× GbE; WiFi 36ms; ROS2 |
| MIC-780 | Intel Core Ultra S2 | LGA1851 | **Integrated NPU**; DDR5 6400; 3× display; DIN rail |
| MIC-785 | AMD Ryzen Emb/EPYC 4005 | AM5 | **First AMD in wiki**; machine vision; iBMC 1.2 |
| mic-7000-series-overview | — | — | Family overview; i-Module GPU options; applications |

---

## Critical MIC-Series Facts

- **MIC-780 = first integrated NPU** in this wiki — Intel Core Ultra AI Boost NPU enables local AI inference without discrete GPU; unique across all ARK + MIC models
- **MIC-785 = first and only AMD** in this wiki — Ryzen Embedded 7000/9000 + EPYC 4005 AM5
- **MIC-760 = only WiFi + ROS2 model** — built for AMR/MMR mobile robots; 3× GbE for camera/LiDAR; CANbus; 36ms WiFi fast roaming
- **MIC-770 V3 ≠ MIC-770**: DDR5 (vs DDR4), NVMe M.2 added, IP40, iBMC 1.2, -20°C start vs -10°C — major upgrade
- **MIC-780W has 4× GbE; MIC-780H has 2× GbE** — same chassis, different chipset (W880 vs H810)
- **i-Module = Advantech modular expansion chassis**: 1/2/4-slot PCIe, storage, GPU modules. MIC-78x uses its own i-Module series (not cross-compatible with MIC-770 i-Modules)
- **MIC-780 minimum power is 12V** (not 9V like MIC-770 series) — matters for battery-powered deployments
- **MIC-760, MIC-7700, MIC-785 have incomplete raw data** — feature lists only, no spec tables; dimensions/RAM/temp missing for these three

---

## ARK Series Key Facts (unchanged from session 5)

- 21 ARK models; see `wiki/synthesis/advantech-ark-series-comparison.md` for full table
- **ARK-7060**: only fan-cooled, AC power, IPMI 2.0, 128GB ECC DDR4, optional 10GbE — server tier
- **ECC memory**: ARK-3532B (DDR4), ARK-3532C (DDR4), ARK-3534D (DDR5), ARK-7060 (DDR4)
- **IEC 62443-4-2 SL2**: ARK-1125C, ARK-3534C, ARK-3534D
- **CAN Bus**: ARK-1125H (2×), ARK-3534C/D (2×), ARK-1221L (1×), ARK-1250L (opt), MIC-760 (1+, unspec.)

---

## Open Questions (unresolved)

- MIC-760 full specs: RAM, temp range lower bound, COM count, CANbus port count, dimensions
- MIC-7700 full specs: temp, dimensions, certifications, DDR spec
- MIC-785 full specs: RAM, display outputs, temp, dimensions, certs
- MIC-780 out-of-band management method (iBMC 1.2 or Intel AMT not specified)
- i-Module cross-generation compatibility matrix (MIC-770 vs MIC-78 series)
- NPU TOPS rating for MIC-780 (Intel Core Ultra AI Boost varies by SKU)
- iBMC 1.2 capability scope: KVM-over-IP or power/sensor only?
- ARK-7060 U0A1 power consumption, certifications still TBD (from prior sessions)

---

## Wiki Structure Reminder

- `index.md` — flat catalog, 73 pages total; read when hotcache is insufficient
- `wiki/synthesis/mic-series-comparison.md` — master MIC comparison (all 8 models)
- `wiki/synthesis/MIC-770x.md` — MIC-7700 → V3 generational hub
- `wiki/synthesis/MIC-78x.md` — MIC-780 vs MIC-785 hub
- `wiki/synthesis/advantech-ark-series-comparison.md` — master ARK comparison (all 21 models)
