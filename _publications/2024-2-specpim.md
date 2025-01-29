---
title: "SpecPIM: Accelerating Speculative Inference on PIM-Enabled System via Architecture-Dataflow Co-Exploration"
collection: publications
permalink: /publications/2024-2-specpim
date: 2024-04-27
venue: 'International Conference on Architectural Support for Programming Languages and Operating Systems (ASPLOS)' 
---
Generative large language models' (LLMs) inference suffers from inefficiency because of the token dependency brought by autoregressive decoding. Recently, speculative inference has been proposed to alleviate this problem, which introduces small language models to generate draft tokens and adopts the original large language model to conduct verification. Although speculative inference can enhance the efficiency of the decoding procedure, we find that it presents variable resource demands due to the distinct computation patterns of the models used in speculative inference. This variability impedes the full realization of speculative inference's acceleration potential in current systems.

To tackle this problem, we propose SpecPIM to accelerate speculative inference on the PIM-enabled system. SpecPIM aims to boost the performance of speculative inference by extensively exploring the heterogeneity brought by both the algorithm and the architecture. To this end, we construct the architecture design space to satisfy each model's disparate resource demands and dedicate the dataflow design space to fully utilize the system's hardware resources. Based on the co-design space, we propose a design space exploration (DSE) framework to provide the optimal design under different target scenarios. Compared with speculative inference on GPUs and existing PIM-based LLM accelerators, SpecPIM achieves 1.52×/2.02× geomean speedup and 6.67×/2.68× geomean higher energy efficiency.

[Download paper here](https://dl.acm.org/doi/abs/10.1145/3620666.3651352)

```
@inproceedings{li2024specpim,
  title={SpecPIM: Accelerating Speculative Inference on PIM-Enabled System via Architecture-Dataflow Co-Exploration},
  author={Li, Cong and Zhou, Zhe and Zheng, Size and Zhang, Jiaxi and Liang, Yun and Sun, Guangyu},
  booktitle={Proceedings of the 29th ACM International Conference on Architectural Support for Programming Languages and Operating Systems, Volume 3},
  pages={950--965},
  year={2024}
}
```