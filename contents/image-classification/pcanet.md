---
id: pcanet
title: 'PCANet: A Simple Deep Learning Baseline for Image Classification
sidebar_label: PCANet'
keywords:
  [
    pcanet,
    pcanet paper,
    a simple deep learning baseline for image classification,
    a simple deep learning baseline,
  ]
---

> Citations: 951 | Paper Published: 14 Apr 2014 | Institutions: MediaTek, University of Macau, ShanghaiTech University, Tsinghua University, Agency for Science, Technology and Research | Authors: Tsung-Han Chan, Kui Jia, Shenghua Gao, Jiwen Lu, Zinan Zeng, Yi Ma

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper proposes a simple deep learning network for image classification called PCA Network (PCANet) which uses cascaded principal component analysis, binary hashing and block-wise histograms. The PCANet model is tested on various benchmark visual datasets and shows competitive results compared to state-of-the-art features.

:::


## Contributions 

The contribution of this paper is the proposal of a simple deep learning network for image classification called PCA Network (PCANet) which uses cascaded principal component analysis, binary hashing and block-wise histograms. The PCANet model shows competitive results compared to state-of-the-art features on various benchmark visual datasets including face recognition tasks with significant illumination changes and corruption. Additionally, two variations to the PCANet are introduced: RandNet and LDANet which share the same topology but have either randomly selected or LDA-learned filters respectively.

## Practical Implications

- The proposed PCA Network (PCANet) provides a simple and efficient deep learning architecture for image classification tasks.
- PCANet can be used as a valuable baseline model to study advanced deep learning architectures for large-scale image classification problems.
- The results obtained from extensive experiments on various benchmark visual datasets demonstrate that the seemingly naive PCANet is competitive with state-of-the-art features, either prefixed or learned by DNNs. 
- This suggests that simpler models like PCANet could potentially reduce computational complexity while maintaining high accuracy in certain applications such as face recognition, texture discrimination, object recognition etc.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

- Cascaded principal component analysis (PCA) to learn multistage filter banks.
- Binary hashing and block histograms for indexing and pooling. 
- Two variations of the PCANet: RandNet which has randomly selected filters, LDANet which learns filters from LDA. 
- Extensive testing on various benchmark visual datasets including face recognition tasks with significant illumination changes and corruption as well as hand-written digit recognition, texture discrimination, object recognition etc.

:::

## Data
- LFW dataset for face verification
- MultiPIE, Extended Yale B, AR and FERET datasets for face recognition
- MNIST dataset for hand-written digits recognition

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

- For face verification task using LFW dataset, PCANet achieved an accuracy rate of 97.45%.
- For face recognition tasks with MultiPIE and Extended Yale B datasets, PCANet obtained a rank-one identification rate of 96.5% and 98%, respectively.
- In FERET database for frontal faces under different illuminations conditions, expressions etc., it achieves a classification accuracy up to %. 
- On MNIST basic dataset for hand-written digits recognition task, the best test error rates were reported by RandNet (), LDAnet() followed by PCAnets which had errors ranging from  percent.

:::


## Limitations

The proposed PCANet model is not suitable for all types of image classification tasks and may require modifications or extensions to achieve better performance in certain applications.



