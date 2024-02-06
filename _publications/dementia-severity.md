---
title: "Dementia Severity Classification under Small Sample Size and Weak Supervision in Thick Slice MRI"
collection: publications
permalink: /publications/dementia-severity/
excerpt: 'we propose to classify the disease severity based on the Fazekas scale through the visual biomarkers, namely the Periventricular White Matter (PVWM) and the Deep White Matter (DWM) changes, in the real-world setting of thick-slice MRI'
date: 2021-03-18
venue: 'ArXiv'
paperurl: 'https://arxiv.org/pdf/2103.10056'
githuburl: 'https://github.com/dementia-classification/Dementia-Severity-Classification'
#citation: "[Bibtex](https://scholar.googleusercontent.com/scholar.bib?q=info:IEhQosxgVZYJ:scholar.google.com/&output=citation&scisdr=ClEwYZ4DEI3rjWJld2Q:AFWwaeYAAAAAZcFjb2TxOycuzGChtDgr_6jJBXk&scisig=AFWwaeYAAAAAZcFjb9lJrPog3gEN3yiY0c5qD7U&scisf=4&ct=citation&cd=-1&hl=en)" 
---
Early detection of dementia through specific biomarkers in MR images plays a critical role in developing support strategies proac- tively. Fazekas scale facilitates an accurate quantitative assessment of the severity of white matter lesions and hence the disease. Imaging Biomark- ers of dementia are multiple and comprehensive documentation of them is time-consuming. Therefore, any effort to automatically extract these biomarkers will be of clinical value while reducing inter-rater discrep- ancies. To tackle this problem, we propose to classify the disease sever- ity based on the Fazekas scale through the visual biomarkers, namely the Periventricular White Matter (PVWM) and the Deep White Mat- ter (DWM) changes, in the real-world setting of thick-slice MRI. Small training sample size and weak supervision in form of assigning severity labels to the whole MRI stack are among the main challenges. To combat the mentioned issues, we have developed a deep learning pipeline that employs self-supervised representation learning, multiple instance learn- ing, and appropriate pre-processing steps. We use pretext tasks such as non-linear transformation, local shuffling, in- and out-painting for self- supervised learning of useful features in this domain. Furthermore, an attention model is used to determine the relevance of each MRI slice for predicting the Fazekas scale in an unsupervised manner. We show the significant superiority of our method in distinguishing different classes of dementia compared to state-of-the-art methods in our mentioned setting, which improves the macro averaged F1-score of state-of-the-art from 61% to 76% in PVWM, and from 58% to 69.2% in DWM.
[Code](https://github.com/dementia-classification/Dementia-Severity-Classification), [Paper](https://arxiv.org/pdf/2103.10056)

