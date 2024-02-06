---
title: "Deep Prompt Tuning for Graph Transformers"
collection: publications
permalink: /publications/deepgpt/
excerpt: 'Prompt tuning for Graph Transformers and Message Passing Graph Neural Networks, improved efficiency and resource utilization of Graph Transformers.'
date: 2023-09-18
venue: 'ArXiv'
paperurl: 'https://arxiv.org/abs/2309.10131'
githuburl: 'https://github.com/rezashkv/DeepGPT'
#citation: "[Bibtex](https://scholar.googleusercontent.com/scholar.bib?q=info:IEhQosxgVZYJ:scholar.google.com/&output=citation&scisdr=ClEwYZ4DEI3rjWJld2Q:AFWwaeYAAAAAZcFjb2TxOycuzGChtDgr_6jJBXk&scisig=AFWwaeYAAAAAZcFjb9lJrPog3gEN3yiY0c5qD7U&scisf=4&ct=citation&cd=-1&hl=en)" 
---
Graph transformers have gained popularity in various graph-based tasks by addressing challenges faced by traditional Graph Neural Networks. However, the quadratic complexity of self-attention operations and the extensive layering in graph transformer architectures present challenges when applying them to graph based prediction tasks. Fine-tuning, a common approach, is resource-intensive and requires storing multiple copies of large models. We propose a novel approach called deep graph prompt tuning as an alternative to fine-tuning for leveraging large graph transformer models in downstream graph based prediction tasks. Our method introduces trainable feature nodes to the graph and pre-pends task-specific tokens to the graph transformer, enhancing the model's expressive power. By freezing the pre-trained parameters and only updating the added tokens, our approach reduces the number of free parameters and eliminates the need for multiple model copies, making it suitable for small datasets and scalable to large graphs. Through extensive experiments on various-sized datasets, we demonstrate that deep graph prompt tuning achieves comparable or even superior performance to fine-tuning, despite utilizing significantly fewer task-specific parameters. Our contributions include the introduction of prompt tuning for graph transformers, its application to both graph transformers and message passing graph neural networks, improved efficiency and resource utilization, and compelling experimental results. This work brings attention to a promising approach to leverage pre-trained models in graph based prediction tasks and offers new opportunities for exploring and advancing graph representation learning.
[Code](https://github.com/rezashkv/DeepGPT), [Paper](https://arxiv.org/abs/2309.10131)

