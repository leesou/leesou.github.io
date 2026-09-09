---
title: "Tetris: Efficient Long-context LLM Serving with Chunkwise Dynamic Sequence Parallelism"
collection: publications
permalink: /publications/2026-2-tetris
date: 2026-06-27
venue: 'International Symposium on Computer Architecture (ISCA)' 
---
With the advancement of large language models (LLMs), their context windows have rapidly expanded. To meet diverse demands from varying-length requests in online services, existing state-of-the-art systems  adjust resource allocation by tuning the sequence parallelism (SP) allocation. However, current dynamic SP allocation lacks flexibility to (1) support stage-specific parallelism requirements in LLM inference, (2) mitigate the global latency degradation from excessive SP allocation, and (3) exploit resource fragments arising from SP size variation. 

To tackle this problem, we propose Chunkwise Dynamic Sequence Parallelism (CDSP), a fine-grained parallelism strategy that assigns SP sizes across \textit{intra-request} token segments. Based on CDSP, we build Tetris, an LLM serving system that (1) efficiently integrates CDSP into disaggregated cluster architecture to satisfy parallelism heterogeneity, (2) dynamically regulates SP size expansion based on real-time load conditions, and (3) adaptively explores chunking plans to utilize fragmented resources while meeting per-request demands. Compared with state-of-the-art systems, Tetris achieves up to 4.35$\times$ lower time-to-first-token (TTFT) under max sustainable loads, reduces median time-between-tokens (TBT) by up to 40.1\%, and increases the max request capacity by up to 45\%.

[Download paper here](https://ieeexplore.ieee.org/abstract/document/11617445)

```
@inproceedings{li2026tetris,
  title={Tetris: Efficient Long-context LLM Serving with Chunkwise Dynamic Sequence Parallelism},
  author={Li, Cong and Yang, Yuzhe and Zheng, Xuegui and Yang, Qifan and Guan, Yijin and Zheng, Size and Chang, Li-Wen and Liu, Shufan and Liu, Xin and Sun, Guangyu},
  booktitle={2026 ACM/IEEE 53rd Annual International Symposium on Computer Architecture (ISCA)},
  pages={1287--1301},
  year={2026},
  organization={IEEE}
}
```
