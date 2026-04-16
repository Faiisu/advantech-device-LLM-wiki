---
title: "Isolated IO"
type: concept
tags: [hardware, embedded, industrial, isolation, safety, electrical]
created: 2026-04-16
updated: 2026-04-16
sources: [ARK-1220F]
---

# Isolated IO

## Definition

I/O interfaces where an electrical barrier (galvanic isolation) is placed between the computer's circuitry and the connected field devices, preventing direct current flow between the two sides. The signal crosses the barrier via transformer, optocoupler, or capacitive coupling. Rated by the breakdown voltage the barrier withstands (e.g., 2.5 kV DC).

## Why It Matters

In industrial environments, ground potential differences between equipment, power surges, and high-frequency electrical noise can damage non-isolated interfaces or corrupt data. Isolation protects both the host computer and the field device, and is often required for safety in power systems, heavy machinery, and outdoor installations.

## Key Properties

- **Isolation voltage:** the maximum sustained voltage across the barrier; ARK-1220F uses **2.5 kV DC**
- **Isolated interfaces typically:** RS-232/422/485 COM ports, GPIO (DI/DO), Ethernet, analog I/O
- **Non-isolated interfaces:** USB is almost never isolated (too complex); power supply input may have its own isolation
- **Physical cost:** isolation circuitry adds board space, cost, and typically power consumption — isolated models are physically wider
- **Application domains:** power distribution, motor drives, industrial machinery, outdoor installations, medical equipment

## ARK-1220F Isolation Profile

The [[ARK-1220F]] provides 2.5 kV DC galvanic isolation on:
- Both GbE ports (Intel i210-IT variant)
- Both COM ports (RS-232/422/485)
- 8-bit GPIO (4DI/4DO)

USB ports are **not** isolated — a known gap for deployments requiring full electrical separation.

## Tensions and Contradictions

- USB is not isolated in ARK-1220F — if a USB-connected device is in the same noisy electrical environment, the protection is incomplete
- Isolation adds to chassis width (ARK-1220F is 60mm wide vs 53.5mm for non-isolated ARK-1220L)

## Related Concepts

[[Industrial IO]], [[Fanless Embedded PC]], [[DIN-Rail Mounting]]

## Sources

[[ARK-1220F]]
