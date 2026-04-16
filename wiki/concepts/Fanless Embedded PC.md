---
title: "Fanless Embedded PC"
type: concept
tags: [hardware, embedded, industrial, thermal, fanless]
created: 2026-04-16
updated: 2026-04-16
sources: [ARK-6322, ARK-3520L, ARK-3532B, ARK-3532C, ARK-3534C, ARK-3534D, ARK-7060]
---

# Fanless Embedded PC

## Definition

An embedded computer that dissipates heat entirely through passive means — typically a metal chassis acting as a heatsink — with no moving parts. Distinct from desktop PCs or server hardware that rely on active cooling fans.

## Why It Matters

Industrial and edge deployments often require hardware that can run continuously in dusty, vibration-prone, or hard-to-access environments. Fans introduce failure points, require maintenance, and cannot tolerate certain environments. Fanless designs trade peak performance for reliability and environmental tolerance.

## Key Properties

- **Passive cooling:** heat conducted through chassis walls; aluminum housing is typical
- **TDP range:** compact models use SoCs in the 5–15W range (e.g., J1900, E3825); expansion box PCs extend this to 45–65W desktop CPUs (e.g., Core i7-6820EQ, Xeon W-1290TE) using larger chassis mass
- **Operating temperature range:** typically -20~60°C with SSD for standard tier; wider (-30~70°C) on some embedded SoCs; narrower with spinning HDDs
- **Vibration and shock ratings:** no mechanical components = better IEC 60068 compliance
- **Airflow dependency:** even passive designs often specify minimum airflow (e.g., 0.7 m/s) for full temperature range

## Product Tiers in This Wiki

| Tier | Form Factor | CPU TDP | Examples |
|---|---|---|---|
| Compact box | ~133×43×94mm, desk/DIN | 5–10W | ARK-1123x, ARK-1124x, ARK-1125x |
| Wide DIN-rail | ~60×158×114mm | 6–20W | ARK-11, ARK-1220x, ARK-1221L, ARK-1250L |
| Slim wall-mount | ~195×55×140mm | ~15W | ARK-1551 |
| Expansion box PC | ~220×101×233mm+ | 45–65W | ARK-3520L, ARK-3532x, ARK-3534x |
| **Extreme performance (fan-cooled)** | 230×205×390mm | 50–67W | ARK-7060 (**NOT fanless** — active cooling) |

## Trade-offs

| Factor | Fanless | With Fans |
|---|---|---|
| Reliability (MTBF) | Higher (no moving parts) | Lower |
| Peak CPU performance | Limited by TDP | Higher |
| Environment tolerance | Dust, vibration, humidity | Controlled environments |
| Maintenance | Near-zero | Periodic fan cleaning |
| Noise | Silent | Audible |

## Related Concepts

[[Industrial IO]], [[Mini PCIe]]

## Sources

[[ARK-6322]]
