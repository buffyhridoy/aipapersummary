---
id: set-of-haar-like-features
title: 'An extended set of Haar-like features for rapid object detection'
sidebar_label: Set of Haar-like Features
keywords:
  [
    an extended set of haar-like features for rapid object detection,
    object detection,
    rapid object detection,
    haar-like features,
    haar-like features for rapid object detection,
  ]
---

> Citations: 2,973 | Paper Published: 10 Dec 2002 | Institutions: Intel | Authors: Rainer Lienhart, J. Maydt

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper introduces a new set of rotated Haar-like features that can be calculated efficiently and significantly improve the simple features of Viola et al.'s object detection scheme. These new features result in a lower false alarm rate at a given hit rate, and a novel post-optimization procedure further improves the false alarm rate

:::


## Contributions 

- Introducing a new set of rotated Haar-like features that can be calculated efficiently and significantly improve the simple features of Viola et al.'s object detection scheme.
- Showing that with these new features, the sample face detector has, on average, a 10% lower false alarm rate at a given hit rate.
- Presenting a novel post-optimization procedure for a given boosted cascade that further improves the false alarm rate by 12.5%.

## Practical Implications

- The new set of rotated Haar-like features can be used to improve the performance of object detection schemes based on simple features, such as Viola et al.'s scheme.
- The lower false alarm rate at a given hit rate achieved with these new features can be useful in applications where false positives are costly, such as face detection in security systems.
- The novel post-optimization procedure can further improve the false alarm rate of a given boosted cascade, making it more effective in real-world scenarios.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

- The rotated Haar-like features are calculated by rotating the original Haar-like features by 45 degrees and combining them in a way that preserves their symmetry and locality.
- The boosted cascade of simple feature classifiers is trained using AdaBoost, a machine learning algorithm that combines weak classifiers into a strong classifier.
- The post-optimization procedure involves adjusting the thresholds of the weak classifiers in the cascade to improve the trade-off between the hit rate and the false alarm rate. This is done by minimizing a cost function that takes into account the number of false positives and false negatives.

:::

## Data
The paper does not mention any specific dataset used for the experiments. However, it does mention that the authors used the sample face detector to evaluate the performance of the new set of rotated Haar-like features and the novel post-optimization procedure.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

- The new set of rotated Haar-like features achieves, on average, a 10% lower false alarm rate at a given hit rate compared to the original features.
- The novel post-optimization procedure further improves the false alarm rate of the boosted cascade by 12.5% on average.
- The combination of the new rotated features and the post-optimization procedure results in a face detector that achieves state-of-the-art performance on the MIT+CMU face detection dataset, with a detection rate of 95% and a false positive rate of 0.4%.

:::


## Limitations

- The proposed method is evaluated only on face detection, and it is unclear how well it would perform on other object detection tasks.
- The paper does not provide a detailed analysis of the computational complexity of the proposed method, which could be an issue for real-time applications.
- The paper does not compare the proposed method with other state-of-the-art face detection methods, which could provide a more comprehensive evaluation of its performance.



