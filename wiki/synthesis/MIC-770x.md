---
title: "MIC-770x Sub-Series Hub"
type: synthesis
tags: [advantech, mic-series, mic-770, comparison, fanless, compact-box]
created: 2026-04-17
updated: 2026-04-17
sources: [MIC-7700, MIC-770, MIC-770-V2, MIC-770-V3]
---

# MIC-770x Sub-Series Hub

**Prompted by:** MIC-series ingest — four generations in the same chassis family
**Type:** Comparison / Selection Guide

## Summary

The MIC-770x line is a four-generation evolution of the same 77×192×230mm compact fanless box PC chassis (plus a wider 107mm variant for V3). Each generation adds approximately one CPU generation, better connectivity, and improved environmental specs. MIC-7700 is the legacy ancestor; MIC-770 V3 is the current mainstream choice.

---

## Comparison Table

| Spec | MIC-7700 | MIC-770 (V1) | MIC-770 V2 | MIC-770 V3 |
|---|---|---|---|---|
| **CPU Socket** | LGA1151 v1 | LGA1151 v2 | LGA1200 | LGA1700 |
| **CPU Gen** | Intel 6th/7th Gen | Intel 8th/9th Gen | Intel 10th Gen Xeon/Core | Intel 12th–14th Gen Core |
| **Chipsets** | Q170 / H110 | Q370 / H310 | W480E / H420E | R680E / H610E |
| **Memory** | DDR4 (unspec.) | DDR4 2400/2666, 64GB | DDR4 2666/2933, 64GB | **DDR5 4800, 128GB** |
| **Storage** | 2.5" + CFast + mSATA | 2.5" + mSATA | 2.5" + mSATA | 2.5" + mSATA + **NVMe M.2** |
| **RAID** | unspec. | Q370: RAID 0/1/5/10 | W480E: RAID 0/1/5/10 | R680E: RAID 0/1/5/10 |
| **Display** | VGA + **DVI** | VGA + HDMI | VGA + HDMI | VGA + HDMI |
| **LAN** | 2× GbE | 2× GbE | 2× GbE | 2× GbE |
| **USB** | 8× USB 3.0 | 4–8× USB 3.x | 4–8× USB 3.2 Gen1/Gen2 | 4–8× USB 3.2 Gen1/Gen2 |
| **COM** | 2× RS-232/422/485 + 4× (cable) | 2× RS-232/422/485 + 4× opt | 2× RS-232/422/485 + 4× opt | 2× RS-232/422/485 + 4× opt |
| **SIM slot** | Yes (mini-PCIe) | No | No | No |
| **CFast** | Yes | No | No | No |
| **Operating Temp** | unspec. (wide) | -10~40°C | -10~50°C | **-20~50°C** |
| **IP Rating** | unspec. | None | None | **IP40** |
| **FlexIO** | No | No | Yes | Yes |
| **iDoor** | No | No | Yes | Yes |
| **RED Compliance** | No | No | Yes | No (not listed) |
| **Out-of-Band Mgmt** | No | No | No | **iBMC 1.2** |
| **vPro/AMT** | Q170 (partial) | Q370 (yes) | W480E (yes) | **Intel vPro/AMT** |
| **TPM** | unspec. | unspec. | unspec. | Supported |
| **Dimensions (W×H×D)** | unspec. | 77×192×230mm | 77×192×230mm | 77×192×230mm (narrow) / 107.3×192×230mm (wide) |
| **Weight** | unspec. | 2.8 kg | 2.8 kg | 2.8 / 4.65 kg |
| **Certs** | unspec. | CE/FCC Class A, CCC, BSMI | unspec. | CE/FCC Class A, CCC, BSMI, UL/CB |

---

## Selection Guide

**Choose MIC-7700** only if you are maintaining an existing installation on this platform (legacy, no new designs recommended).

**Choose MIC-770 (V1)** only if 8th/9th Gen supply availability and cost are primary drivers — otherwise V2 or V3 is superior on every dimension.

**Choose MIC-770 V2** if:
- RED compliance is required for EU deployment
- Azure PnP or AWS IoT Greengrass ecosystem certification is needed
- 10th Gen Xeon W (with ECC via W480E) is required for reliability
- Budget is tighter than V3

**Choose MIC-770 V3** if:
- DDR5, NVMe M.2, or PCIe Gen4 storage performance is needed
- Operating environment starts below -10°C (-20°C rating)
- IP40 dust protection is needed
- Out-of-band management (iBMC 1.2) is required
- Intel vPro/AMT or TPM is required without additional modules
- Latest CPU generation (12th–14th Gen) is preferred for AI workloads or longevity

---

## Confidence

High — spec tables fully available for V1/V2/V3; MIC-7700 has limited raw data (feature list only).

## Gaps and Open Questions

- MIC-7700 operating temperature, dimensions, and certifications not confirmed
- V1 GPIO module support (likely via iDoor-style expansion, unconfirmed)
- V2 certifications not listed in raw
- iBMC 1.2 feature scope (KVM-over-IP vs power/sensor only) unconfirmed

## Sources Used

[[MIC-7700]], [[MIC-770]], [[MIC-770-V2]], [[MIC-770-V3]]
