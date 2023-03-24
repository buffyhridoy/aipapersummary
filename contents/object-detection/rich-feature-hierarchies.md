---
id: rich-feature-hierarchies
title: 'Rich Feature Hierarchies for Accurate Object Detection and Semantic Segmentation'
sidebar_label: Rich Feature Hierarchies
keywords:
  [
    rich feature hierarchies,
    rich feature hierarchies for accurate object detection and semantic segmentation,
    accurate object detection,
    semantic segmentation,
  ]
---

> Citations: 15,107 | Paper Published: 23 Jun 2014 | Institutions: University of California, Berkeley | Authors: Ross Girshick, Jeff Donahue, Trevor Darrell, Jitendra Malik

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

This paper proposes a simple and scalable object detection algorithm that combines high-capacity CNNs with supervised pre-training for an auxiliary task, followed by domain-specific fine-tuning. The proposed method outperforms previous methods on the PASCAL VOC 2012 dataset.

:::


## Contributions 

The contributions of this paper are the two key insights that improve object detection performance: (1) applying high-capacity convolutional neural networks to bottom-up region proposals and (2) supervised pre-training for an auxiliary task, followed by domain-specific fine-tuning. These approaches are combined to give a simple and scalable algorithm that outperforms previous methods by more than 30%.

## Practical Implications

The practical implications of this paper are that it presents a simple and scalable object detection algorithm that outperforms previous methods by more than 30%. This can have significant impact in various fields such as computer vision, robotics, autonomous vehicles etc. where accurate object detection is crucial for decision making. The proposed method also provides insight into what the network learns which could be useful for further research on deep learning models.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

- Combining high-capacity convolutional neural networks (CNNs) with bottom-up region proposals to localize and segment objects.
- Using supervised pre-training for an auxiliary task, followed by domain-specific fine-tuning when labeled training data is scarce. This approach yields a significant performance boost.
- The proposed method combines region proposals with CNN features which is called R-CNN: Regions with CNN features.

:::

## Data
The data used in this paper is the PASCAL VOC 2012 dataset, which is a widely-used benchmark for object detection. The dataset contains images with annotations of objects belonging to twenty different classes such as person, car, dog etc. This allows researchers to evaluate and compare their algorithms on a standardized set of images and metrics.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

The results of the paper show that the proposed method outperforms previous state-of-the-art approaches by more than 30% on PASCAL VOC 2012 dataset, achieving a mean average precision (mAP) score of 53.3%. The experiments also provide insight into what the network learns and reveal a rich hierarchy of image features. Table 1 in the paper shows complete results on VOC 2010 where they compare their method against four strong baselines including SegDPM which combines DPM detectors with semantic segmentation system output and uses additional inter-detector context and image-classifier rescoring.

:::


## Limitations

- The proposed method is computationally expensive and requires a lot of memory, which makes it difficult to use on low-end devices.
- The dataset used in the experiments (PASCAL VOC 2012) only contains images with annotations for twenty different object classes. This limits the generalizability of the results to other datasets or real-world scenarios where more diverse objects may be present.


