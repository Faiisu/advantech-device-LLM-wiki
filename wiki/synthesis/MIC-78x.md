---
title: "MIC-78x Sub-Series Hub"
type: synthesis
tags: [advantech, mic-series, mic-780, mic-785, comparison, fanless, npu, amd]
created: 2026-04-17
updated: 2026-04-17
sources: [MIC-780, MIC-785]
---

# MIC-78x Sub-Series Hub

**Prompted by:** MIC-series ingest — two new-generation compact box PCs sharing a design philosophy
**Type:** Comparison / Selection Guide

## Summary

The MIC-78x line (MIC-780 and MIC-785) represents Advantech's latest compact fanless box PCs, sharing the 195×80×240mm chassis footprint and one-side IO cabling design. MIC-780 offers Intel Core Ultra Series 2 with integrated NPU; MIC-785 is the first AMD option, targeting machine vision with AMD's Radeon integrated graphics and EPYC-class multi-core performance.

---

## Comparison Table

| Spec | MIC-780 | MIC-785 |
|---|---|---|
| **CPU Architecture** | Intel Core Ultra 5/7/9 (Series 2) | AMD Ryzen Embedded 7000/9000 / EPYC 4005 |
| **Socket** | LGA1851 | AM5 (LGA1718) |
| **TDP** | Up to 65W | Not specified |
| **Cores** | Up to 24 | Varies by SKU |
| **Chipset** | Intel W880 / H810 | Not specified |
| **Memory** | DDR5 6400MHz, 128GB max | DDR5 (speed/capacity not specified) |
| **NPU** | Yes — Intel Xe LPG + AI Boost NPU | No (AMD iGPU handles AI inference) |
| **iGPU** | Intel Xe LPG | AMD Radeon RDNA 3 |
| **Storage** | 2× 2.5" HDD/SSD + 1× NVMe M.2 + 1× mini-PCIe | 2× 2.5" HDD/SSD + 1× NVMe M.2 |
| **Display** | 3× (1× DP + 2× HDMI) | Multiple (types/count unspecified) |
| **LAN (W/H SKU)** | W880: 4× GbE; H810: 2× GbE | Not specified |
| **COM** | 2× RS-232/422/485 + 4× opt | Not specified (GbE, USB, COM listed as present) |
| **Operating Temp** | -20~50°C with airflow | Not specified |
| **Power Input** | 12~36 VDC | 12~36 VDC |
| **Mounting** | Desktop / Wall / DIN rail | Not specified |
| **Dimensions** | 195 × 80 × 240 mm | Not specified (aligns with MIC-770/780 design) |
| **i-Module** | MIC-78 series i-Module | i-Module supported |
| **FlexIO** | Not listed | Yes |
| **iDoor** | Not listed | Yes |
| **iBMC** | Not confirmed | iBMC 1.2 confirmed |
| **Certs** | CE/FCC Class A, CCC, BSMI, UL/CB | Not listed |

---

## Selection Guide

**Choose MIC-780** if:
- On-device AI inference via integrated NPU is a requirement (avoids discrete GPU cost and power)
- Triple simultaneous display output is needed (1× DP + 2× HDMI)
- 4× GbE is needed (MIC-780W variant)
- DIN rail mounting is required alongside desktop/wall options
- Intel ecosystem (OpenVINO, Intel AMT) is preferred

**Choose MIC-785** if:
- AMD Radeon integrated GPU performance is preferred for machine vision (better FP16/INT8 per watt vs Intel Xe in some workloads)
- AMD EPYC 4005 multi-core density is required for high-thread-count control workloads
- AMD ecosystem (ROCm, OpenCL) is required for existing software
- iBMC 1.2 out-of-band management is confirmed needed (listed for MIC-785; not confirmed for MIC-780)

---

## Confidence

Medium — MIC-780 has a complete spec table; MIC-785 has only a feature list. Comparison is partially based on architectural knowledge rather than confirmed spec data.

## Gaps and Open Questions

- MIC-785 full spec table missing (RAM, display, LAN count, temp, dimensions)
- MIC-780 iBMC / Intel AMT out-of-band management not specified
- MIC-78 series i-Module compatibility with MIC-770 i-Modules unconfirmed
- MIC-785 NPU capability: AMD EPYC 4005 and Ryzen 7000/9000 do not have a dedicated NPU block (unlike Intel Core Ultra); AI inference falls to iGPU or CPU

## Sources Used

[[MIC-780]], [[MIC-785]]
