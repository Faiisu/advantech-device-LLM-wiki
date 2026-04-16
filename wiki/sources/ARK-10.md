---
title: "ARK-10"
type: source
tags: [hardware, embedded, industrial-pc, fanless, advantech, j1900]
created: 2026-04-16
updated: 2026-04-16
sources: [self]
---

# ARK-10

**Type:** Product Specification Sheet  
**Author(s):** Advantech  
**Origin:** `raw/ARK-10.md` | https://www.advantech.com/th-th/products/1-2jkbyz/ark-10/

## Summary

Compact fanless box PC based on the Intel Celeron J1900. Notable for having 2 GB RAM and a 500 GB 2.5" 24×7 SATA HDD **built-in** — one of the few ARK models that ships with storage and memory pre-installed. Dual Intel i210 GbE NICs (Wake on LAN). Minimal I/O profile compared to other ARK-1000 series members.

## Key Specs

- **CPU:** Intel Celeron J1900 (Bay Trail), 4-core, 2.0 GHz (burst 2.41 GHz)
- **Memory:** DDR3 1333 MHz, up to 8 GB, 1× SO-DIMM; **2 GB built-in**
- **Display:** 1× VGA only
- **Ethernet:** 2× Intel i210 GbE (Wake on LAN)
- **Serial:** 2× RS-232/422/485 (BIOS selectable)
- **USB:** 1× USB 3.0 + 2× USB 2.0
- **Storage:** 1× 500 GB 2.5" 24×7 SATA HDD built-in; 1× half-size mSATA
- **Expansion:** 1× full-size Mini PCIe (WLAN); 1× half-size Mini PCIe (mSATA)
- **Power:** 12 VDC; 36W adapter; threaded DC jack
- **Operating temp:** 0–50°C (0.7 m/s airflow)
- **Dimensions:** 133.8 × 43.1 × 94.2 mm; aluminum housing
- **Mounting:** VESA / DIN Rail / Wall (optional kits)
- **OS:** WES7, Windows 7/8; Linux by project
- **Certifications:** UL 62368, CB, CCC, BSMI; CE/FCC Class A; **no RED**

## Differentiators vs. ARK Series

- Built-in 2 GB RAM and 500 GB HDD — deploy-ready out of box
- Intel i210 GbE (better than RTL8111E in ARK-6322)
- Only 1× VGA display output — limited for modern display use

## Entities Mentioned

[[Advantech]], [[Intel Celeron J1900]]

## Concepts Introduced or Elaborated

[[Fanless Embedded PC]], [[Industrial IO]], [[Mini PCIe]]

## Connections to Existing Wiki

- Same J1900 CPU as [[ARK-6322]] but smaller form factor (133.8×43.1 vs 200×64×200 mm) and fewer COM ports (2 vs 6)
- Uses Intel i210 GbE vs Realtek RTL8111E in ARK-6322 — more enterprise-grade NIC

## Open Questions

- Why only VGA and no HDMI — is this an older product?
- 24×7 rated HDD suggests always-on deployment — what application class?
