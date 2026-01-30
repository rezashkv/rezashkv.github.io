---
title: "Catalog-Native LLM: Speaking Item-ID dialect with Less Entanglement for Recommendation"
collection: publications
permalink: /publications/idiomoe/
excerpt: 'IDIOMoE decouples item-ID and language processing inside an LLM via token-type MoE, reducing interference and improving recommendation quality at roughly the same compute'
date: 2026-01-25
venue: 'ICLR 2026'
venueurl: 'https://openreview.net/forum?id=ia9vDh0Ltn'
paperurl: 'https://arxiv.org/abs/2510.05125'
githuburl: 'https://github.com//rezashkv'
authors: 'Reza Shirkavand, Xiaokai Wei, Chen Wang, Zheng Hui, Heng Huang, Michelle Gong'
figure: '/images/idiomoe.jpeg' 
highlight: true
---
While collaborative filtering delivers predictive accuracy and efficiency, and Large Language Models (LLMs) enable expressive and generalizable reasoning, modern recommendation systems must bring these strengths together. Growing user expectations, such as natural-language queries and transparent explanations, further highlight the need for a unified approach. However, doing so is nontrivial. Collaborative signals are often token-efficient but semantically opaque, while LLMs are semantically rich but struggle to model implicit user preferences when trained only on textual inputs. This paper introduces Item-ID + Natural-language Mixture-of-Experts Language Model (IDIOMoE), which treats item interaction histories as a native dialect within the language space, enabling collaborative signals to be understood in the same way as natural language. By splitting the Feed Forward Network of each block of a pretrained LLM into a separate text expert and an item expert with token-type gating, our method avoids destructive interference between text and catalog modalities. IDIOMoE demonstrates strong recommendation performance across both public and proprietary datasets, while preserving the text understanding of the pretrained model.
[Code](https://github.com//rezashkv), [Paper](https://arxiv.org/abs/2510.05125), [ICLR 2026](https://openreview.net/forum?id=ia9vDh0Ltn)

