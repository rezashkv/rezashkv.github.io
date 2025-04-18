---
title: "Efficient Fine-Tuning and Concept Suppression for Pruned Diffusion Models"
collection: publications
permalink: /publications/ft-unlearn/
excerpt: 'How to train a small diffusion model while suppressing unwanted concepts'
date: 2024-12-19
venue: 'CVPR 2025'
venueurl: 'https://cvpr.thecvf.com/Conferences/2025/AcceptedPapers'
paperurl: 'https://arxiv.org/abs/2412.15341'
githuburl: 'https://github.com/rezashkv/diffusion_pruning'
authors: 'Reza Shirkavand, Peiran Yu, Shangqian Gao, Gowthami Somepalli, Tom Goldstein, Heng Huang'
figure: '/images/ft-unlearn.png' 
---
Recent advances in diffusion generative models have yielded remarkable progress. While the quality of generated content continues to improve, these models have grown considerably in size and complexity. This increasing computational burden poses significant challenges, particularly in resource-constrained deployment scenarios such as mobile devices. The combination of model pruning and knowledge distillation has emerged as a promising solution to reduce computational demands while preserving generation quality. However, this technique inadvertently propagates undesirable behaviors, including the generation of copyrighted content and unsafe concepts, even when such instances are absent from the fine-tuning dataset. In this paper, we propose a novel bilevel optimization framework for pruned diffusion models that consolidates the fine-tuning and unlearning processes into a unified phase. Our approach maintains the principal advantages of distillation-namely, efficient convergence and style transfer capabilities-while selectively suppressing the generation of unwanted content. This plug-in framework is compatible with various pruning and concept unlearning methods, facilitating efficient, safe deployment of diffusion models in controlled environments.
[Code](https://github.com/rezashkv/diffusion_pruning), [Paper](https://arxiv.org/abs/2412.15341),

