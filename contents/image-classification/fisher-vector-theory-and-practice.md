---
id: fisher-vector-theory-and-practice
title: 'Image Classification with the Fisher Vector: Theory and Practice'
sidebar_label: Fisher Vector Theory and Practice
keywords:
    [
    fisher vector,
    image classification,
    fisher vector representation,
    fisher vector theory and practice,
    fisher vector theory and practice paper,
    Image Classification with the Fisher Vector

    ]
---

> Citations: 1,501 | Paper Published: 01 Dec 2013 | Institutions: National University of Cordoba, Xerox, University of Amsterdam, French Institute for Research in Computer Science and Automation | Authors: Jorge Sanchez, Florent Perronnin, Thomas Mensink, Jakob Verbeek

<!-- Prettier doesn't change this -->

:::tip Abstract in 2 Lines

The paper proposes a new patch encoding strategy called Fisher Vector (FV) for image classification and retrieval. The FV framework describes patches by their deviation from an "universal" generative Gaussian mixture model, which is efficient to compute and leads to excellent results even with linear classifiers.

:::

## Contributions

The main contribution of this paper is the proposal of a new patch encoding strategy called Fisher Vector (FV) for image classification and retrieval. The FV framework describes patches by their deviation from an "universal" generative Gaussian mixture model, which leads to excellent results even with linear classifiers while being efficient to compute. Additionally, experimental results on five standard datasets demonstrate that the proposed approach outperforms existing methods such as Bag-of-Visual words representation across various metrics like mean average precision (mAP).

## Practical Implications

The practical implications of this paper are that the proposed Fisher Vector (FV) framework can be used as an alternative patch encoding strategy for image classification and retrieval. The FV approach is efficient to compute, leads to excellent results even with linear classifiers, and can be compressed using product quantization without significant loss of accuracy. This makes it a promising technique for real-world applications where efficiency and accuracy are important factors. Additionally, experimental results on five standard datasets demonstrate its superiority over existing methods such as Bag-of-Visual words representation across various metrics like mean average precision (mAP).

## Methods

<!-- Prettier doesn't change this -->

:::info Methodology

The main method used in this paper is the Fisher Vector (FV) framework, which describes patches by their deviation from an "universal" generative Gaussian mixture model. The authors also compare FV with other existing methods such as Bag-of-Visual words representation and Super Vectors (SV). Additionally, they conduct experiments on five standard datasets to evaluate the performance of FV across various metrics like mean average precision (mAP).

:::

## Data
The authors of this paper have used five standard datasets to evaluate the performance of their proposed Fisher Vector (FV) framework. These datasets include PASCAL VOC 2007, Caltech 256, SUN 397, ILSVRC 2010 and ImageNet10K. They conduct experiments on these datasets to demonstrate that FV outperforms existing methods such as Bag-of-Visual words representation across various metrics like mean average precision (mAP).

## Results

<!-- Prettier doesn't change this -->

:::note Performance Analysis

- On the PASCAL VOC dataset with a vocabulary size of K=64 using linear SVMs for classification: FV achieves mAP =72.1%, while BoW obtains only mAP =58%
 
- On the Caltech101 dataset with a vocabulary size of K=128 using non-linear kernel SVMs for classification: FV achieves accuracy rate at top one is around ~90% whereas SV achieved an accuracy rate at top one is about ~80%.

:::

## Limitations

Limitation of this paper is that it focuses on the use of Fisher Vectors (FVs) for image classification and retrieval tasks, but does not explore their potential applications in other areas such as object detection or semantic segmentation.
