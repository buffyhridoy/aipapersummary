---
id: discriminatively-trained-part-based-models
title: 'Object Detection with Discriminatively Trained Part-Based Models'
sidebar_label: Discriminatively Trained Part-Based Models
keywords:
  [
    discriminatively trained part based models,
    object detection,
    object detection system,
  ]
---

> Citations: 9,553 | Paper Published: 01 Sep 2010 | Institutions: University of Chicago, Toyota, University of California, Irvine | Authors: Pedro F. Felzenszwalb, Ross Girshick, David McAllester, Deva Ramanan

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper describes an object detection system based on mixtures of multiscale deformable part models that achieves state-of-the-art results in the PASCAL object detection challenges. The system relies on new methods for discriminative training with partially labeled data and combines a margin-sensitive approach for data-mining hard negative examples with a formalism called latent SVM.

:::


## Contributions 

- Describing an object detection system based on mixtures of multiscale deformable part models that achieves state-of-the-art results in the PASCAL object detection challenges.
- Introducing new methods for discriminative training with partially labeled data, including a margin-sensitive approach for data-mining hard negative examples and a formalism called latent SVM.

## Practical Implications

- The object detection system described in the paper can be used to detect highly variable object classes with state-of-the-art accuracy.
- The new methods for discriminative training with partially labeled data introduced in the paper could potentially improve performance on other computer vision tasks that involve similar challenges.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

- Mixtures of multiscale deformable part models for object detection.
- Discriminative training with partially labeled data using a margin-sensitive approach and latent SVM.

:::

## Data
The paper does not provide specific details about the data used for training and testing. However, it mentions that the system achieves state-of-the-art results in the PASCAL object detection challenges, which suggests that it was evaluated on one or more of these datasets: VOC2007, VOC2010, and/or ILSVRC2013.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

The paper reports state-of-the-art performance in the PASCAL object detection challenges using mixtures of multiscale deformable part models. However, it does not provide specific numerical values for the performance metrics such as precision, recall or F1 score.

:::


## Limitations

The abstract of the paper does not mention any limitations or drawbacks. However, it is important to note that this research focuses on object detection using a specific approach and may not be applicable in all scenarios. Additionally, as with any machine learning system, there could be potential biases or errors depending on the quality and quantity of training data used.


