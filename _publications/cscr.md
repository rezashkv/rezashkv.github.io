---
title: "Cost-Aware Contrastive Routing for LLMs"
collection: publications
permalink: /publications/cscr/
excerpt: 'CSCR embeds both prompts and LLMs into a shared space using fast logit or perplexity fingerprints. A cost‑banded InfoNCE loss trains the space to balance quality against cost. It generalizes to unseen models and out‑of‑distribution prompts.'
date: 2025-09-18
venue: 'NeurIPS 2025 Spotlight'
venueurl: 'https://neurips.cc'
paperurl: 'https://arxiv.org/pdf/2508.12491'
githuburl: 'https://github.com/rezashkv/cscr'
authors: 'Reza Shirkavand, Shangqian Gao, Peiran Yu, Heng Huang'
figure: '/images/cscr.png' 
highlight: true
---
We study cost-aware routing for large language models across diverse and dynamic pools of models. Existing approaches often overlook prompt-specific context, rely  on expensive model profiling, assume a fixed set of experts, or use inefficient trial-and-error strategies. We introduce Cost-Spectrum Contrastive Routing (CSCR), a  lightweight framework that maps both prompts and models into a shared embedding  space to enable fast, cost-sensitive selection. CSCR uses compact, fast-to-compute  logit footprints for open-source models and perplexity fingerprints for black-box APIs. A contrastive encoder is trained to favor the cheapest accurate expert within adaptive cost bands. At inference time, routing reduces to a single k-NN lookup via a FAISS index, requiring no retraining when the expert pool changes and enabling microsecond latency. Across multiple benchmarks, CSCR consistently outperforms baselines, improving the accuracy–cost tradeoff by up to 25%, while generalizing robustly to unseen LLMs and out-of-distribution prompts.
[Code](https://github.com/rezashkv/cscr), [Paper](https://arxiv.org/pdf/2508.12491),

