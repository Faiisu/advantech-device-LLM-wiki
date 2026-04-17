---
title: "SUSIAccess"
type: concept
tags: [software, advantech, embedded, api, management]
created: 2026-04-16
updated: 2026-04-17
sources: [ARK-1123H, MIC-770, MIC-770-V2, MIC-770-V3, MIC-7700, MIC-780, MIC-785]
---

# SUSIAccess

## Definition

Advantech's embedded software management layer and API suite for local hardware feature access. Provides standardized control of watchdog timer, GPIO, thermal monitoring, backlight, and other platform-specific features via a unified cross-platform API (also called SUSI API in newer documentation).

## Why It Matters

Standardizes hardware feature access across Advantech product families, allowing application software to control hardware functions without low-level driver development. Eliminates need to port platform-specific code when switching between Advantech models.

## Key Properties

- Exposed via SUSI API (Standardized Unified System Interface) — used interchangeably with SUSIAccess in newer Advantech documentation
- Features accessible: watchdog timer, GPIO, fan control, thermal monitoring, backlight, OSD
- Available on both ARK and MIC series
- Appears alongside DeviceOn: SUSI/SUSIAccess handles local hardware access; DeviceOn handles remote cloud management

## Relationship to DeviceOn

SUSIAccess/SUSI API handles local hardware abstraction; [[DeviceOn]] (WISE-DeviceOn) handles remote management, OTA updates, and cloud integration. They are complementary layers, not mutually exclusive. MIC-series documentation uses "SUSI API" terminology; ARK-series uses "SUSIAccess" — same underlying concept.

## Sources

[[ARK-1123H]], [[MIC-7700]], [[MIC-770]], [[MIC-770-V2]], [[MIC-770-V3]], [[MIC-780]], [[MIC-785]]
