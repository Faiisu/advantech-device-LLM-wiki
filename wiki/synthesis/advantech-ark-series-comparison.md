---
title: "Advantech ARK Series Comparison"
type: synthesis
tags: [hardware, embedded, advantech, comparison, industrial-pc]
created: 2026-04-16
updated: 2026-04-16
sources: [ARK-6322, ARK-10, ARK-11, ARK-1123C, ARK-1123H, ARK-1123L, ARK-1124C, ARK-1124H, ARK-1125C, ARK-1125H, ARK-1220F, ARK-1220L, ARK-1221L, ARK-1250L, ARK-1551, ARK-3520L, ARK-3532B, ARK-3532C, ARK-3534C, ARK-3534D, ARK-7060]
---

# Advantech ARK Series Comparison

**Prompted by:** Batch ingest of ARK-1000/1200/1500 series spec sheets alongside ARK-6322.  
**Type:** Comparison table + key selection dimensions

## Summary

The Advantech ARK series spans from Bay Trail-era J1900 (2014) to 14th Gen Core (2023) and Xeon D-1700 (2021), covering compact box PCs, DIN-rail nodes, slim wall-mount computers, expansion box PCs, and server-grade extreme performance boxes. The ARK-7000 tier (ARK-7060) is distinct from all others: fan-cooled, AC power input, IPMI 2.0, and up to 128GB ECC DDR4 with optional 10GbE.

---

## Master Comparison Table

| Model | CPU | Platform | Cores | RAM | Display | LAN | COM | CAN | USB | GPIO | Op Temp | Power (typ) | Form | RED | Special |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| ARK-6322 | J1900 | Bay Trail | 4 | 8GB DDR3L | VGA+DP | 2×GbE | 6×RS | — | 1×USB3+7×USB2 | 8-bit | 0–50°C | 15.7W | Box 200×64×200mm | No | 6 COM ports |
| ARK-10 | J1900 | Bay Trail | 4 | 8GB DDR3 | VGA | 2×i210 GbE | 2×RS | — | 1×USB3+2×USB2 | — | 0–50°C | — | Box 133×43×94mm | No | Built-in HDD+RAM |
| ARK-1123C | E3825 | Bay Trail-M | 2 | 8GB DDR3L | VGA | 2×i210 GbE | 2×RS | — | 1×USB3+2×USB2 | — | **-30–70°C** | 5.28W | Box 133×43×94mm | No | FCC Class B, DeviceOn |
| ARK-1123H | J1900 | Bay Trail | 4 | 8GB DDR3L | 2×HDMI | 2×i210 GbE | 2×RS | — | 1×USB3+2×USB2 | — | -20–60°C | 5.64W | Box 133×43×94mm | Option | SUSIAccess |
| ARK-1123L | E3825 | Bay Trail-M | 2 | 8GB DDR3L | VGA | 1×i210 GbE | 1×RS-232+1×RS | — | 1×USB3+1×USB2 | 8-bit | **-30–70°C** | 5.28W | Box 133×43×94mm | No | FCC Class A, GPIO, 2×mPCIe |
| ARK-11 | N3350 | Apollo Lake | 2 | 8GB DDR3L | 2×HDMI 4K | 2×i210 GbE | 2×RS | — | 4×USB3 | 8-bit opt | -30–70°C | 6.4W | DIN 53×158×114mm | No | Widest temp, DeviceOn |
| ARK-1124C | N3350 | Apollo Lake | 2 | 8GB DDR3L | VGA | 1×GbE | 4×RS | — | 2×USB3 | — | -20–60°C | 5.5W | DIN 133×46×94mm | No | 4 COM, iDoor, single GbE |
| ARK-1124H | E3940 | Apollo Lake | 4 | 8GB DDR3L | 2×HDMI 4K | 2×GbE | 1×RS | — | 4×USB3 | — | -20–60°C | 6.02W | DIN 133×46×94mm | Option | TPM 2.0, iDoor |
| ARK-1220F | E3940 | Apollo Lake | 4 | 8GB DDR3L | HDMI+VGA | 2×i210 isolated | 2×RS isolated | — | 4×USB3+1×USB2 | 8-bit isolated | -30–60°C | TBD | DIN 60×158×114mm | No | 2.5kV isolation |
| ARK-1220L | E3940 | Apollo Lake | 4 | 8GB DDR3L | 2×HDMI 4K | 2×i210 GbE | 2×RS | — | 4×USB3 | 8-bit | -30–70°C | 7.6W | DIN 53×158×114mm | No | -30–70°C, WISE-PaaS |
| ARK-1221L | x6413E/J6412/N6210 | Elkhart Lake | 2–4 | 32GB DDR4 | HDMI+DP 4K | 2×i225 2.5G | 2×RS | 1× | 2×USB3.2+2×USB2 | 8-bit | -40–60°C | 9.6W | DIN 60×158×114mm | No | -40°C, 32GB, HDMI+DP |
| ARK-1125C | x7211E | Alder Lake-N | 4 | 16GB DDR5 | 1×HDMI | 1×i226 2.5G | 4×RS | — | 2×USB3.2+2×USB2 | 8-bit | -30–60°C | 10.05W | DIN 133×46×94mm | No | DDR5, IEC 62443-4-2 |
| ARK-1125H | N200 | Alder Lake-N | 4 | 16GB DDR5 | 2×HDMI 4K | 2×i226 2.5G | 2×RS | 2× | 2×USB3.2+2×USB2 | 8-bit | -30–60°C | 10.54W | DIN 133×46×94mm | Yes | 2×CAN, dual 2.5GbE |
| ARK-1250L | Core i3/i5-11th | Tiger Lake | 2–4 | 64GB DDR4 | HDMI+VGA | 3–4×GbE mix | 4×RS | opt | 2×USB3.2+2×USB2 | 8-bit | -40–60°C | 18–20W | DIN 60×173×141mm | No | Highest performance, 64GB |
| ARK-1551 | Core i5-8th/Celeron | Whiskey Lake | 2–4 | 32GB DDR4 | HDMI+VGA | 2×GbE | 4×RS | — | 4×USB3.1 Gen2 | 8-bit | -20–55°C | 9–14W | Slim 195×55×140mm | Yes | Swappable bay, NVMe, RAID |
| ARK-3520L | Core i5/i7-6th (BGA) | Skylake-H | 4 | 32GB DDR4 | VGA+HDMI+opt 3rd | 2×GbE | 8×RS | — | 6×USB3+2×USB2 | 16-bit | -20–60°C | 11.4–68.4W | Box 220×101×233mm | No | AMO-3xxx riser, iDoor, 8 COM |
| ARK-3532B | Xeon W / Core i-10th | Comet Lake-S/W | 2–10 | 64GB DDR4 ECC | VGA+HDMI+opt 3rd | 4×GbE | 6×RS | — | 8×USB3 | 16-bit | -20–60°C | 30W typ/64.8W max | Box (dims TBD) | No | PCIe x16 GPU slot, TPM 2.0 |
| ARK-3532C | Xeon W / Core i-10th | Comet Lake-S/W | 2–10 | 64GB DDR4 ECC | VGA+HDMI+opt 3rd | 4×GbE | 4–6×RS | — | 8×USB3 | 16-bit | -20–60°C | 30W typ/64.8W max | Box (dims TBD) | No | 2× PCI legacy, no PCIe x16 |
| ARK-3534C | Core i3/i5/i7/i9-12/13/14th | Raptor Lake | 4–24 | 64GB DDR5 | 2×HDMI+opt 3rd | 2×GbE (1×2.5G) | 4–6×RS | 2× | 4×USB3+4×USB2 | 16-bit | TBD | TBD | Box (dims TBD) | No | DDR5, IEC 62443-4-2 SL2, no ECC |
| ARK-3534D | Core i3/i5/i7/i9-12/13/14th | Raptor Lake | 4–24 | 64GB DDR5 ECC | 2×HDMI+opt 3rd | 4×GbE (3×2.5G) | 4–6×RS | 2× | 8×USB3 | 16-bit | TBD | TBD | Box (dims TBD) | No | DDR5 ECC, IEC 62443-4-2 SL2, 4× GbE |
| ARK-7060 | Xeon D-1746TER/D-1715TER | Ice Lake-D | 4–10 | **128GB DDR4 ECC** | VGA (BMC) | 2×GbE+opt 2×10GbE | — | — | 4×USB3 | — | **-10–50°C** | 62.7W(U4A1)/TBD | Box 230×205×390mm | No | **Fan-cooled, AC power, IPMI 2.0**, 350W GPU slot |

---

## Key Selection Dimensions

### By Operating Temperature
| Requirement | Best Choice |
|---|---|
| -40°C | ARK-1221L (x6413E), ARK-1250L |
| -30°C | **ARK-1123C, ARK-1123L**, ARK-11, ARK-1220F, ARK-1220L, ARK-1125C, ARK-1125H |
| -20°C | ARK-1123H, ARK-1124C, ARK-1124H, ARK-1551, ARK-3520L, ARK-3532B, ARK-3532C |
| -10°C (active cooling required) | ARK-7060 (0.7m/s airflow) |
| 0°C minimum | ARK-6322, ARK-10 |
| TBD (spec sheet incomplete) | ARK-3534C, ARK-3534D |

### By COM Port Count
| COM Count | Models |
|---|---|
| 8× COM | ARK-3520L |
| 6× COM | ARK-6322, ARK-3532B, ARK-3532C (00A1) |
| 4–6× COM | ARK-3534C, ARK-3534D (4 base + 2 optional) |
| 4× COM | ARK-1124C, ARK-1125C, ARK-1250L, ARK-1551, ARK-3532C (00A1U) |
| 2× COM | ARK-10, ARK-11, ARK-1123C, ARK-1123H, ARK-1124H, ARK-1125H, ARK-1220F, ARK-1220L, ARK-1221L |
| 2× COM (mixed RS-232+RS) | ARK-1123L |
| 1× COM | ARK-1124H |

### By CAN Bus
| CAN Count | Models |
|---|---|
| 2× CAN | ARK-1125H, ARK-3534C, ARK-3534D |
| 1× CAN | ARK-1221L, ARK-1250L (optional) |
| No CAN | All others |

### By RED Certification
| Status | Models |
|---|---|
| Certified / available | ARK-1125H, ARK-1551 |
| Available via optional module | ARK-1123H (AMO-WIFI08E), ARK-1124H (AMO-WIFI10, single-layer only) |
| No RED | ARK-6322, ARK-10, ARK-11, ARK-1124C, ARK-1125C, ARK-1220F, ARK-1220L, ARK-1221L, ARK-1250L |

### By Memory Capacity
| Max RAM | Models |
|---|---|
| **128 GB DDR4 ECC** | **ARK-7060** |
| 64 GB DDR5 ECC | ARK-3534D |
| 64 GB DDR5 | ARK-3534C |
| 64 GB DDR4 ECC | ARK-3532B, ARK-3532C |
| 64 GB DDR4 | ARK-1250L |
| 32 GB DDR4 | ARK-1221L, ARK-1551, ARK-3520L |
| 16 GB DDR5 | ARK-1125C, ARK-1125H |
| 8 GB | ARK-6322, ARK-10, ARK-11, ARK-1123H, ARK-1124C, ARK-1124H, ARK-1220F, ARK-1220L |

### By IEC 62443-4-2 SL2
| Status | Models |
|---|---|
| Certified | ARK-1125C, ARK-3534C, ARK-3534D |
| Not certified | All others |

### By Isolated IO
| Isolation | Models |
|---|---|
| 2.5 kV DC (GbE + COM + GPIO) | ARK-1220F |
| None | All others |

---

## Generation Timeline

```
Bay Trail (2013-2014):        J1900 (Bay Trail-D) — ARK-6322, ARK-10, ARK-1123H
                              E3825 (Bay Trail-M) — ARK-1123C, ARK-1123L
Skylake-H (2015):             Core i5-6440EQ, i7-6820EQ — ARK-3520L [ARK-3000 tier]
Apollo Lake (2016-2017):      N3350, E3940 — ARK-11, ARK-1124C, ARK-1124H, ARK-1220F, ARK-1220L
Whiskey Lake (2018):          Core i5-8365UE — ARK-1551
Comet Lake-S/W (2020):        Xeon W-1290TE / Core i-10th — ARK-3532B, ARK-3532C [ARK-3000 tier]
Elkhart Lake (2021):          x6413E/J6412/N6210 — ARK-1221L
Tiger Lake (2021):            Core i5-1145G7E — ARK-1250L
Alder Lake-N (2023):          x7211E, N200 — ARK-1125C, ARK-1125H
Alder/Raptor Lake LGA1700:    12/13/14th Gen 65W — ARK-3534C, ARK-3534D [ARK-3000 tier]
Xeon D-1700 (Ice Lake-D 2021): D-1715TER/D-1746TER 50–67W — ARK-7060 [ARK-7000 tier, fan-cooled, AC power]
```

---

## Confidence

High — all data drawn directly from Advantech spec sheets in `raw/`.

## Gaps and Open Questions

- ARK-1123C and ARK-1123L specs unavailable (cookie wall) — stubs created
- Power consumption not available for ARK-1220F
- CAN Bus version (2.0A/B/FD) not specified in any model
- Which iDoor modules are compatible with each ARK — needs Advantech iDoor catalog ingest
- Shock ratings vary by source and are not consistently listed — omitted from table

## Sources Used

[[ARK-6322]], [[ARK-10]], [[ARK-11]], [[ARK-1123C]], [[ARK-1123H]], [[ARK-1123L]], [[ARK-1124C]], [[ARK-1124H]], [[ARK-1125C]], [[ARK-1125H]], [[ARK-1220F]], [[ARK-1220L]], [[ARK-1221L]], [[ARK-1250L]], [[ARK-1551]], [[ARK-3520L]], [[ARK-3532B]], [[ARK-3532C]], [[ARK-3534C]], [[ARK-3534D]], [[ARK-7060]]
