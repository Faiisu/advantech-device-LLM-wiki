---
title: "NPU"
type: concept
tags: [npu, ai, inference, intel, core-ultra, edge-ai]
created: 2026-04-17
updated: 2026-04-17
sources: [MIC-780, mic-7000-series-overview]
---

# NPU

## Definition

A Neural Processing Unit (NPU) is a dedicated hardware accelerator integrated into a processor die, optimized for matrix operations and inference workloads characteristic of neural networks. Unlike a GPU (general-purpose parallel compute) or CPU (serial logic), an NPU is purpose-built for low-power, high-throughput AI inference tasks.

## Why It Matters

NPUs enable on-device AI inference without requiring a discrete GPU, dramatically reducing power consumption, cost, and form factor. In industrial embedded systems, this means edge AI workloads (object detection, anomaly detection, predictive maintenance) can run on a fanless box PC rather than requiring a server-class or GPU-equipped system.

## Key Properties

- Integrated into the processor die (vs discrete GPU add-in card)
- Optimized for INT8/INT4 matrix operations common in neural network inference
- Performance measured in TOPS (Tera Operations Per Second)
- Intel Core Ultra Series 2 integrates an NPU alongside the CPU and Intel Xe LPG GPU
- Works in conjunction with OpenVINO (Intel), ONNX Runtime, and other inference frameworks
- Does not replace GPU for training workloads; complement to, not replacement for, discrete GPU

## Evidence and Examples

- [[MIC-780]] is described by Advantech as "the first fanless industrial box PC powered by Intel Core Ultra Processors with integrated NPU"
- Intel Core Ultra Series 2 (Meteor Lake) includes the Intel AI Boost NPU, rated at 13 TOPS (NPU-only) in consumer variants; industrial spec may differ
- MIC-7 series GPU i-Modules (MIC-75G20/G30) support discrete NVIDIA GPUs up to 350W for training-adjacent or heavy inference — complementary, not competing with NPU use case

## Tensions and Contradictions

- TOPS ratings for Intel Core Ultra NPU vary widely across SKUs (U-series vs H-series); the MIC-780 spec sheet does not specify which Core Ultra SKU or its NPU TOPS rating.
- NPU vs GPU for industrial inference: NPU is efficient for sustained low-batch inference; GPU i-Modules remain necessary for high-batch or multi-stream vision workloads.

## Related Concepts

[[i-Module]], [[Fanless Embedded PC]], [[AMR MMR]]

## Sources

[[MIC-780]], [[mic-7000-series-overview]]
