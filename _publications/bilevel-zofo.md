---
title: "Bilevel ZOFO: Bridging Parameter-Efficient and Zeroth-Order Techniques for Efficient LLM Fine-Tuning and Meta-Training"
collection: publications
permalink: /publications/bilevel-zofo/
excerpt: 'We propose Bilevel ZOFO, a novel bilevel optimization framework that bridges parameter-efficient and zeroth-order optimization techniques for efficient large language model (LLM) fine-tuning and meta-training.'
date: 2025-02-05
venue: 'ArXiv'
paperurl: 'https://www.arxiv.org/abs/2502.03604'
githuburl: 'https://github.com/Peiran225/bilevel_ZOFO'
authors: 'Reza Shirkavand, Qi He, Peiran Yu, Heng Huang'
figure: '/images/bilevel-zofo.png' 
---
Fine-tuning pre-trained Large Language Models (LLMs) for downstream tasks using First-Order (FO) optimizers presents significant computational challenges. Parameter-Efficient Fine-Tuning(PEFT) methods have been proposed to address these challenges by freezing most model parameters and training only a small subset. While PEFT is efficient, it may not outperform full fine-tuning when high task-specific performance is required. Zeroth-Order (ZO) methods offer an alternative for fine-tuning the entire pre-trained model by approximating gradients using only the forward pass, thus eliminating the computational burden of back-propagation in first-order methods. However, when implementing ZO methods, a hard prompt is crucial, and relying on simple, fixed hard prompts may not be optimal. In this paper, we propose a bilevel optimization framework that complements ZO methods with PEFT to mitigate sensitivity to hard prompts while efficiently and effectively fine-tuning LLMs. Our Bilevel ZOFO (Zeroth-Order-First-Order) method employs a double-loop optimization strategy, where only the gradient of the PEFT model and the forward pass of the base model are required. We provide convergence guarantees for Bilevel ZOFO. Empirically, we demonstrate that Bilevel ZOFO outperforms both PEFT and ZO methods in single-task settings while maintaining similar memory efficiency. Additionally, we show its strong potential for multitask learning. Compared to current first-order meta-training algorithms for multitask learning, our method has significantly lower computational demands while maintaining or improving performance.
[Code](https://github.com/Peiran225/bilevel_ZOFO), [Paper](https://www.arxiv.org/abs/2502.03604)

