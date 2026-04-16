---
updated: 2026-04-16
session: 5
---

# Hotcache

> Rolling summary of recent wiki activity (~500 words max). Read this before index.md or any wiki file. If the answer is here, skip further reads. Overwrite entirely each update — do not append.

---

## Wiki Domain

This wiki is exclusively about **Advantech ARK-series industrial and edge PCs** (fanless box PCs, DIN-rail computers, expansion box PCs, and server-grade extreme performance PCs). All non-Advantech content has been removed.

---

## What Has Been Ingested (21 sources total)

**Advantech ARK hardware (21 models):**

| Model | CPU | Form | Key Trait |
|---|---|---|---|
| ARK-6322 | J1900 | Box | 6× COM, 200×64mm |
| ARK-10 | J1900 | Box | Built-in 2GB RAM + 500GB HDD |
| ARK-1123C | E3825 | Box | Dual GbE, -30~70°C, FCC Class B |
| ARK-1123H | J1900 | Box | Dual HDMI, SUSIAccess, RED option |
| ARK-1123L | E3825 | Box | Single GbE, 8-bit GPIO, FCC Class A, -30~70°C |
| ARK-11 | N3350 | DIN-rail | -30~70°C, DeviceOn, 12–28V |
| ARK-1124C | N3350 | DIN-rail | 4× COM, single GbE, iDoor |
| ARK-1124H | E3940 | DIN-rail | Dual HDMI 4K, TPM 2.0, iDoor |
| ARK-1125C | x7211E | DIN-rail | DDR5, 4× COM, IEC 62443-4-2 SL2 |
| ARK-1125H | N200 | DIN-rail | DDR5, 2× CAN Bus, dual 2.5GbE, RED |
| ARK-1220F | E3940 | DIN-rail | 2.5 kV isolated GbE+COM+GPIO |
| ARK-1220L | E3940 | DIN-rail | Dual HDMI 4K, -30~70°C, WISE-PaaS |
| ARK-1221L | x6413E | DIN-rail | DDR4 32GB, -40°C, 1× CAN |
| ARK-1250L | Core i5-11th | DIN-rail | 64GB DDR4, triple GbE, 4× COM, -40°C |
| ARK-1551 | Core i5-8th | Slim wall | Swappable bay, RAID, NVMe, RED |
| ARK-3520L | Core i5/i7-6th BGA | Expansion box | 8× COM, triple display, iDoor |
| ARK-3532B | Xeon W / Core i-10th | Expansion box | PCIe x16 GPU slot, ECC DDR4, TPM 2.0 |
| ARK-3532C | Xeon W / Core i-10th | Expansion box | 2× PCI legacy, ECC DDR4, 4× GbE |
| ARK-3534C | Core i-12/13/14th | Expansion box | DDR5, 2× CAN, IEC 62443-4-2 SL2, no ECC |
| ARK-3534D | Core i-12/13/14th | Expansion box | DDR5 ECC, 2× CAN, IEC 62443-4-2 SL2, 4× GbE |
| **ARK-7060** | **Xeon D-1746TER / D-1715TER** | **Extreme perf box** | **Fan-cooled, AC power, IPMI 2.0, 128GB ECC DDR4, opt 10GbE** |

---

## Key Facts to Remember

- **ARK-7060 = completely different tier:** Only model with active cooling (fans), AC power (100–240V), and IPMI 2.0 server management. -10~50°C requires 0.7m/s airflow. 230×205×390mm, 9.7kg.
- **ARK-7060 has no COM ports** — only ARK without RS-232/422/485.
- **128GB DDR4 ECC (ARK-7060)** — highest in wiki; 4× SO-DIMM, Xeon D-1700 SoC.
- **Optional 10GbE:** ARK-7060 via AMO-I031 (Intel X550) — only 10GbE model in wiki.
- **PCIe x16 GPU slot:** ARK-3532B and ARK-7060 — ARK-7060 supports up to 350W GPU.
- **ECC memory:** ARK-3532B (DDR4), ARK-3532C (DDR4), ARK-3534D (DDR5), ARK-7060 (DDR4 128GB).
- **IEC 62443-4-2 SL2:** ARK-1125C, ARK-3534C, ARK-3534D.
- **CAN Bus (2×):** ARK-1125H, ARK-3534C, ARK-3534D. CAN (1×): ARK-1221L, ARK-1250L (opt).
- **ARK-3534C/D spec sheets** are sparse — no operating temperature or power consumption listed.

---

## Open Questions (unresolved)

- ARK-7060 U0A1 (10-core) power consumption: TBD in spec sheet
- ARK-7060 COM ports: genuine absence or spec sheet omission?
- ARK-7060 certifications not listed in spec sheet
- ARK-3534C/D operating temperature: unconfirmed
- CAN Bus version (2.0A/B/FD): unspecified across all models
- ARK-3532C EMC/safety certification: missing from spec sheet

---

## Wiki Structure Reminder

- `index.md` — flat catalog of all 52 pages; read this when hotcache is insufficient
- `wiki/synthesis/advantech-ark-series-comparison.md` — master comparison table, all 21 ARK models
- `wiki/synthesis/ARK-1123x.md`, `ARK-1124x.md`, `ARK-1125x.md` — ARK-1000 sub-series hubs
- `wiki/synthesis/ARK-3532x.md`, `ARK-3534x.md` — ARK-3000 sub-series hubs
