---
id: in-defense-of-nearest-neighbor
title: 'In defense of Nearest-Neighbor based image classification'
sidebar_label: In Defense of Nearest-Neighbor
keywords:
  [
    in defense of nearest-neighbor,
    nearest neighbor,
    nearest neighbor based image classification,
    nearest neighbor based image classifier,
    nearest neighbor based image classification,
  ]    
---

> Citations: 1,180 | Paper Published: 23 Jun 2008 | Institutions: Weizmann Institute of Science, Adobe Systems | Authors: Oren Boiman, E. Shechtman, Michal Irani

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper proposes a non-parametric nearest-neighbor (NN) based image classifier that requires no training time and performs better than traditional NN-based classifiers. The proposed algorithm, NBNN, computes direct 'image-to-class' distances without descriptor quantization and ranks among the top leading learning-based image classifiers.

:::


## Contributions 

The main contribution of this paper is the proposal of a non-parametric nearest-neighbor (NN) based image classifier, NBNN, that performs better than traditional NN-based classifiers and ranks among the top leading learning-based image classifiers. The authors argue that two commonly used practices in image classification - descriptor quantization and computation of 'image-to-image' distance instead of 'image-to-class' distance - have led to inferior performance for nonparametric methods. They propose an algorithm that requires no descriptor quantization and computes direct 'image-to-class' distances without training time or intensive learning stages using SVM or Boosting algorithms. Empirical comparisons are shown on several challenging databases including Caltech-101 ,Caltech-256, and Graz-01 datasets.

## Practical Implications

- The proposed NBNN algorithm provides a simple and efficient image classification method that requires no training time.
- It performs better than traditional non-parametric nearest neighbor (NN) based classifiers, which require intensive learning/training stages using SVM or Boosting methods.
- By computing direct 'image-to-class' distances without descriptor quantization, the performance gap between NN-based and learning-based image classifiers is reduced considerably. 
- Empirical comparisons on several challenging databases show that NBNN ranks among the top leading learning-based image classifiers. 


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

The paper proposes a non-parametric nearest-neighbor (NN) based image classifier, NBNN. The algorithm computes direct 'image-to-class' distances without descriptor quantization and requires no training time or intensive learning stages using SVM or Boosting algorithms. Empirical comparisons are shown on several challenging databases including Caltech-101 ,Caltech-256, and Graz-01 datasets to demonstrate the effectiveness of this method compared to traditional NN-based classifiers as well as leading learning-based image classifiers.

:::

## Data
The paper uses several challenging databases to evaluate the performance of the proposed NBNN algorithm. These include Caltech-101, Caltech-256, and Graz-01 datasets commonly used in computer vision research for image classification tasks.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

- On the Caltech 101 dataset, NBNN achieved an accuracy rate of 91%, which is comparable with other state-of-the-art methods such as Spatial Pyramid Matching Kernel (SPMK), but with much less computational complexity than SPMK.
 
- Similarly, on the larger-scale Caltech 256 dataset containing more objects per category than in CalTech 101 database; NBNN outperformed all previous published results by achieving an overall recognition rate of over ~80%.

- Finally,on Graz01 data set that contains six different classes including airplanes cars faces motorbikes watches. NBNN was able to achieve better performance when compared against existing machine-learning techniques like Support Vector Machines(SVMs).

:::


## Limitations

- The proposed NBNN algorithm assumes the Naive-Bayes assumption, which may not hold in all cases.
- The authors argue that descriptor quantization and computation of 'image-to-image' distance have led to inferior performance for nonparametric methods, these practices may still be useful in certain contexts where computational complexity is less important than accuracy.



