---
title: Pac-PIM: A Parallel Communication Framework for Commodity Processing-in-memory Systems
collection: publications
permalink: /publications/2025-5-pacpim
date: 2025-12-16
venue: 'Transactions on Architecture and Code Optimization (TACO)' 
---
Processing-in-memory (PIM) is a promising paradigm to effectively alleviate the bottleneck of memory access for memory-intensive applications. UPMEM PIM-enabled DIMMs, the first commercially available PIM platform integrating processing elements (PEs) in DIMMs, exemplifies this trend. However, the communication overhead between the host and PIM-enabled DIMMs remains significant. Although previous studies have attempted to reduce this overhead between the host and PIM-enabled DIMMs, our detailed investigation reveals that, from the software perspective, the native communication framework fails to fully leverage its parallelism for communication.

We propose to combine rank-level parallelism and process-level parallelism in the layered fashion to take advantage of these and avoid their respective drawbacks. And we revamp the native communication framework by integrating this combination to introduce Pac-PIM (Parallel Communication Framework for PIM). Our evaluation, conducted using real UPMEM PIM-enabled DIMMs and representative PIM-enabled applications, shows that Pac-PIM significantly improves communication performance in all scenarios, with an average speedup of 1.53× compared to the native communication framework with excellent scalability. In addition, Pac-PIM can further improve communication performance along with other optimizations.

[Download paper here](https://dl.acm.org/doi/full/10.1145/3776751)

```
@article{yang2025pac,
  title={Pac-PIM: A Parallel Communication Framework for Commodity Processing-in-memory Systems},
  author={Yang, Fan and Zhou, Zhe and Li, Cong and Ho, Tsung-Yi and Yang, Ming-Chang},
  journal={ACM Transactions on Architecture and Code Optimization},
  year={2025},
  publisher={ACM New York, NY}
}
```