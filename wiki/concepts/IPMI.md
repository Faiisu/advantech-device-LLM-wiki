---
title: "IPMI"
type: concept
tags: [hardware, server, management, bmc, out-of-band, embedded]
created: 2026-04-16
updated: 2026-04-16
sources: [ARK-7060]
---

# IPMI

## Definition

**Intelligent Platform Management Interface (IPMI)** is a standardized hardware-level management interface that operates independently of the host CPU and OS. It enables remote monitoring, control, and recovery of a server or embedded PC via a dedicated management network port, even when the system is powered off or unresponsive. IPMI 2.0 is the current standard version, adding enhanced security (RAKP encryption, role-based access) and Serial over LAN (SOL).

## Why It Matters

In this wiki, IPMI represents the boundary between embedded industrial PCs (ARK-1000/3000 series, managed via DeviceOn/SUSIAccess over the main network) and server-grade edge computing (ARK-7060, managed via IPMI out-of-band). IPMI is essential for mission-critical deployments where remote power cycling, firmware flashing, or bare-metal OS reinstallation must be possible without physical access.

## Key Properties

- **BMC (Baseboard Management Controller):** Dedicated microcontroller that runs IPMI firmware; in ARK-7060, this is the **Aspeed AST2500**
- **Dedicated management port:** Separate GbE port isolated from data network; ARK-7060 has 1× dedicated management port
- **Out-of-band (OOB):** Functions independently of host OS; accessible when system is powered down (standby power required)
- **IPMI 2.0 features:** Remote power on/off/reset, hardware sensor monitoring (temp, fan, voltage), event logging (SEL), virtual KVM, Serial over LAN (SOL), PXE boot support
- **VGA via BMC:** ARK-7060 routes its VGA output through the AST2500 BMC, enabling remote display access

## Evidence and Examples

- [[ARK-7060]]: IPMI 2.0-compliant; Aspeed AST2500 BMC; 1× dedicated GbE management port; VGA output via BMC

## Tensions and Contradictions

- No other ARK model in this wiki supports IPMI — it is exclusive to the ARK-7000 series as represented here.
- ARK-1000/3000 series use [[DeviceOn]] for remote management, which operates over the main network and requires OS-level agents — fundamentally different from IPMI's hardware-level OOB access.

## Related Concepts

[[DeviceOn]], [[SUSIAccess]]

## Sources

[[ARK-7060]]
