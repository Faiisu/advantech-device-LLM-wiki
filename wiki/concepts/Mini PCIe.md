---
title: "Mini PCIe"
type: concept
tags: [hardware, embedded, expansion, interface]
created: 2026-04-16
updated: 2026-04-16
sources: [ARK-6322]
---

# Mini PCIe

## Definition

A compact PCIe expansion slot standard used in embedded and mobile systems. Supports full-size and half-size cards. Commonly used to add WLAN, WWAN (LTE/5G), mSATA storage, or other peripherals to small-form-factor systems.

## Why It Matters

Provides flexible expansion in platforms where a full PCIe slot is impractical. A key enabler of modularity in embedded PCs — the same base board can support different wireless, storage, or I/O configurations via Mini PCIe.

## ARK-6322 Configuration

- **Slot 1 (full-size):** supports mSATA storage module or WWAN module (note: mSATA shares this slot — mutually exclusive)
- **Slot 2 (half-size):** supports WLAN module

## Related Concepts

[[Fanless Embedded PC]], [[Industrial IO]]

## Sources

[[ARK-6322]]
