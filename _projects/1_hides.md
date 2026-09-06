---
layout: page
title: HiDeS — Diffusion LLM Acceleration
description: Algorithm–system co-design that accelerates block-diffusion LLM inference through hierarchical delta sparsity.
img:
importance: 1
category: research
---

**Advisor:** Prof. Celine Lin, Georgia Tech &nbsp;·&nbsp; **Jan 2026 – present**
&nbsp;·&nbsp; *Under review at HPCA '26*

HiDeS is an algorithm–system co-design approach that exploits hierarchical sparsity to
accelerate block-diffusion model inference through **selective recomputation** across three
granularities — layer, token, and column.

- Built custom **CUDA** kernels for attention and MLP to support selective recomputation.
- Developed on top of the **Fast-dLLM v2** block-diffusion model.
- Achieved **2.33× and 2.67× speedups** on NVIDIA A100 and H100 GPUs respectively.
