---
title: "ARGUS: Hallucination and Omission Evaluation in Video-LLMs"
collection: publications
permalink: /publications/argus/
excerpt: 'An evaluation framework and benchmark for free-form video-LLMs hallucination and omission.'
date: 2025-06-10
venue: 'ICCV 2025'
venueurl: 'https://iccv.thecvf.com/Conferences/2025/AcceptedPapers'
paperurl: 'https://arxiv.org/abs/2506.07371'
githuburl: 'https://huggingface.co/datasets/tomg-group-umd/argus'
authors: 'Ruchit Rawal, Reza Shirkavand, Heng Huang, Gowthami Somepalli, Tom Goldstein'
figure: '/images/argus.png' 
highlight: true
---
Video large language models have not yet been widely deployed, largely due to their tendency to hallucinate. Typical benchmarks for Video-LLMs rely simply on multiple-choice questions. Unfortunately, VideoLLMs hallucinate far more aggressively on freeform text generation tasks like video captioning than they do on multiple choice verification tasks. To address this weakness, we propose ARGUS, a VideoLLM benchmark that measures freeform video captioning performance. By comparing VideoLLM outputs to human ground truth captions, ARGUS quantifies dual metrics. First, we measure the rate of hallucinations in the form of incorrect statements about video content or temporal relationships. Second, we measure the rate at which the model omits important descriptive details. Together, these dual metrics form a comprehensive view of video captioning performance.
[Code](https://github.com/JARVVVIS/argus), [Paper](https://arxiv.org/abs/2506.07371),

