---
title: "Helios: Enabling Dynamic KV Cache Management for Near-Memory Processing via Hybrid-Bonding-based 3D-DRAM"
collection: publications
permalink: /publications/2026-3-helios
date: 2026-10-31
venue: 'International Symposium on Microarchitecture (MICRO)' 
---
Large language models (LLMs) have been widely deployed for online generative services, where numerous LLM instances jointly handle requests with fluctuating  arrival rates and variable request lengths. To efficiently execute coexisting compute-intensive and memory-intensive operators, near-memory processing (NMP) based computing paradigm has been extensively proposed. However, existing NMP designs adopt coarse-grained KV cache management and inflexible attention execution flow. Such limitations hinder these proposals from efficiently handling highly dynamic LLM serving workloads, limiting their ability to accelerate LLM serving. 

To tackle these problems, we propose HeLios, a Hybrid-bonding-based LLM Serving accelerator. Helios aims to bridge the fundamental gap between dynamic KV cache management in LLM serving and the distributed, non-uniform memory abstraction among NMP processing engines (PEs). To this end, we design both the hardware architecture and operator execution for distributed tiled attention execution. We further propose spatially-aware KV cache allocation mechanism to balance the attention workload distribution while minimizing the inter-PE data transfer overhead. Compared with existing GPU/NMP designs, Helios achieves 3.25× (geomean) speedup and 3.36× (geomean) better energy efficiency, along with $\ge$72\%/76\% P50/P99 time-between-tokens reduction.
