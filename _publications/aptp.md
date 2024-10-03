---
title: "Not All Prompts Are Made Equal: Prompt-based Pruning of Text-to-Image Diffusion Models"
collection: publications
permalink: /publications/aptp/
excerpt: 'Dynamic Prompt-based Pruning of Text-to-Image Diffusion Models'
date: 2024-06-17
venue: 'ArXiv'
paperurl: 'https://arxiv.org/abs/2406.12042'
githuburl: 'https://github.com/rezashkv/diffusion_pruning'
authors: 'Reza Shirkavand, Alireza Ganjdanesh, Shangqian Gao, Heng Huang'
#citation: "[Bibtex](https://scholar.googleusercontent.com/scholar.bib?q=info:ZkCwRc5-7bgJ:scholar.google.com/&output=citation&scisdr=ClExa795EPesk0nPEiI:AFWwaeYAAAAAZv7JCiJJwHMa3sda3gsFkNG24VI&scisig=AFWwaeYAAAAAZv7JCuMjfKl65zI00CI_v1C_Qlk&scisf=4&ct=citation&cd=-1&hl=en)" 
---
Text-to-image (T2I) diffusion models have demonstrated impressive image generation capabilities. Still, their computational intensity prohibits resource-constrained organizations from deploying T2I models after fine-tuning them on their internal target data. While pruning techniques offer a potential solution to reduce the computational burden of T2I models, static pruning methods use the same pruned model for all input prompts, overlooking the varying capacity requirements of different prompts. Dynamic pruning addresses this issue by utilizing a separate sub-network for each prompt, but it prevents batch parallelism on GPUs. To overcome these limitations, we introduce Adaptive Prompt-Tailored Pruning (APTP), a novel prompt-based pruning method designed for T2I diffusion models. Central to our approach is a prompt router model, which learns to determine the required capacity for an input text prompt and routes it to an architecture code, given a total desired compute budget for prompts. Each architecture code represents a specialized model tailored to the prompts assigned to it, and the number of codes is a hyperparameter. We train the prompt router and architecture codes using contrastive learning, ensuring that similar prompts are mapped to nearby codes. Further, we employ optimal transport to prevent the codes from collapsing into a single one. We demonstrate APTP's effectiveness by pruning Stable Diffusion (SD) V2.1 using CC3M and COCO as target datasets. APTP outperforms the single-model pruning baselines in terms of FID, CLIP, and CMMD scores. Our analysis of the clusters learned by APTP reveals they are semantically meaningful. We also show that APTP can automatically discover previously empirically found challenging prompts for SD, e.g., prompts for generating text images, assigning them to higher capacity codes.
[Code](https://github.com/rezashkv/diffusion_pruning), [Paper](https://arxiv.org/abs/2406.12042)
