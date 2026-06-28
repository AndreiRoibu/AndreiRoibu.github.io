---
title: "From Cloud To Edge: Three Key Enablers for LLMs on Smart Glasses"
excerpt: "The transformative power of LLMs is undeniable, but the real challenge is bringing them to resource-constrained edge devices such as smart glasses."
layout: single
header:
  image: /assets/images/smart_glasses.jpeg
  teaser: /assets/images/smart_glasses.jpeg
  caption: "Photo credit: [Pexels](https://pexels.com)"
category: "AI"
section: blog
tags:
  - LLM
  - Embedded Systems
  - Deep-Tech
  - Algorithm Optimisation
author_profile: true
read_time: true
toc: true
toc_sticky: true
toc_label: "On This Page"
toc_icon: "fa fa-stream"
original_date: 2025-08-01
---

<div class="notice--info" markdown="1">
The transformative power of LLMs is undeniable, but the real challenge is bringing them to resource-constrained edge devices.
</div>

## Smart Glasses Cannot Exist Without LLMs

_**Why would anyone buy smart glasses when they already have a smartphone that does it all?**_. The answer is the promise of a seamless, hands-free, private AI assistant, packaged in a sleek, lightweight, and stylish design.

The core challenge is that large language models (LLMs) consist of billions of parameters, requiring not only a large memory footprint, but also significant computational resources to run (see [Section 2.2.3 of my PhD Thesis](https://ora.ox.ac.uk/objects/uuid:a792835e-dac8-4241-978a-97c95085feb5)). By design, edge devices like smart glasses are resource- and area-constrained, with limited processing power, memory, and battery life. This situation opens a resource gap, forcing large AI models to the cloud, creating a series of challenges, from high latency to privacy concerns.

## The Solution is as Simple as 1, 2, 3

Bridging this gap is a story in three parts.

### 1. We Start by Making Models Smaller: Compression & Optimisation



First, we shrink the model without compromising its performance. Techniques such as quantisation (using lower-precision numbers), pruning (removing redundant weights), and knowledge distillation (training a smaller model to mimic a larger one) can drastically reduce an LLM's size. For instance, methods like [eDKM clustering](https://www.mdpi.com/2076-3417/15/9/4632) have already compressed LLaMA models from over 12 GB to a more manageable 2.5 GB with minimal impact on performance.

### 2. We Then Make Them Smarter: Efficient Inference

Second, we make the model run more efficiently. The biggest bottleneck in modern computing is not the computation, but the slow and energy-intensive act of moving data between memory and the processor, which can be up to [100x slower and more power-hungry](https://knowen-production.s3.amazonaws.com/uploads/attachment/file/5270/10.1038_s41565-020-0655-z.pdf). Several key innovations can help with this problem:
* **[FlashAttention](https://arxiv.org/abs/2205.14135)**: A re-engineered attention mechanism that uses operation tiling to reduce the number of memory accesses;
* **[KV Caching](https://huggingface.co/blog/not-lain/kv-caching)**: A technique that reuses Key/Value matrices computed previously, by caching them in memory and reusing them.
* **[Grouped-Query Attention (GQA)](https://arxiv.org/pdf/2305.13245)**: An upgrade to KV Caching, which reduces the number of Key-Value pairs we need to store in memory by grouping several heads to share a single Key-Value pair, leading to reduced data movements and memory usage.

### 3. Finally, We Upgrade the Hardware: Next-Generation Edge Devices

Finally, the hardware itself is evolving. We are seeing a new generation of chips emerging, such as the **[Qualcomm AR1 Gen 1](https://www.qualcomm.com/products/mobile/snapdragon/xr-vr-ar/snapdragon-ar1-plus-gen-1-platform)** and the **[Apple Neural Engine](https://machinelearning.apple.com/research/neural-engine-transformers)**, explicitly designed to run complex AI models at the edge. Designers often pair these chips with **High-Bandwidth Memory** technologies like [LPDDR5X](https://semiconductor.samsung.com/dram/lpddr/lpddr5x/), designed for fast data access on power-constrained devices.

Yet, even these do not solve the fundamental data movement bottleneck. Addressing this situation is where novel concepts like In-Memory Computing (IMC) come into play, which perform computations directly in the memory. You can read more about this in a [case study on IMC in LLM Accelerators](https://synthara.ai/research/computeram-in-ai-accelerators-an-llm-case-study/).

## Truly Personal AI Assistants Require a Multidisciplinary Approach

Deploying LLMs on edge devices is a multidisciplinary challenge that demands innovation across the entire stack, from model compression to novel hardware. The industry is closing the gap by advancing in these three areas, enabling the dream of running powerful, private AI assistants on resource-constrained devices like smart glasses, seamlessly integrating them into our daily lives.
