---
title: "Incomplete Multimodal Learning for Complex Brain Disorders Prediction"
collection: publications
permalink: /publications/incomplete-mm/
excerpt: 'We propose a new incomplete multimodal data integration approach that employs transformers and generative adversarial networks to effectively exploit auxiliary modalities available during training in order to improve the performance of a unimodal model at inference.'
date: 2023-05-25
venue: 'ArXiv'
paperurl: 'https://arxiv.org/pdf/2305.16222'
githuburl: 'https://github.com/rezashkv/incomplete-mm'
authors: 'Reza Shirkavand, Heng Huang'
#citation: "[Bibtex](https://scholar.googleusercontent.com/scholar.bib?q=info:IEhQosxgVZYJ:scholar.google.com/&output=citation&scisdr=ClEwYZ4DEI3rjWJld2Q:AFWwaeYAAAAAZcFjb2TxOycuzGChtDgr_6jJBXk&scisig=AFWwaeYAAAAAZcFjb9lJrPog3gEN3yiY0c5qD7U&scisf=4&ct=citation&cd=-1&hl=en)" 
---
Recent advancements in the acquisition of various brain data sources have created new opportunities for integrating multimodal brain data to assist in early detection of complex brain disorders. However, current data integration approaches typically need a complete set of biomedical data modalities, which may not always be feasible, as some modalities are only available in large-scale research cohorts and are prohibitive to collect in routine clinical practice. Especially in studies of brain diseases, research cohorts may include both neuroimaging data and genetic data, but for practical clinical diagnosis, we often need to make disease predictions only based on neuroimages. As a result, it is desired to design machine learning models which can use all available data (different data could provide complementary information) during training but conduct inference using only the most common data modality. We propose a new incomplete multimodal data integration approach that employs transformers and generative adversarial networks to effectively exploit auxiliary modalities available during training in order to improve the performance of a unimodal model at inference. We apply our new method to predict cognitive degeneration and disease outcomes using the multimodal imaging genetic data from Alzheimer's Disease Neuroimaging Initiative (ADNI) cohort. Experimental results demonstrate that our approach outperforms the related machine learning and deep learning methods by a significant margin.
[Code](https://github.com/rezashkv/incomplete-mm), [Paper](https://arxiv.org/pdf/2305.16222)

