---
id: yolov4
title: 'YOLOv4: Optimal Speed and Accuracy of Object Detection'
sidebar_label: YOLOv4
keywords:
  [
    yolov4,
    object detection,
    object detection in cluttered scenes,
    multiscale intensity differences,
    adjacent regions,
    support vector machine classifier,
    car detection,
    driver assistance system,
    robotics,
    driver assistance systems,
    real world scenarios,
    real time application,
    person detection system,
    object recognition,
    feature extractor,
    computer vision tasks,
    object detection system,
    object class,
    large set of positive and negative examples,
    support vector machine classifier,
    overcomplete dictionary of local,
    multiscale intensity differences between adjacent regions,
    car detection tasks,
    real time application of the person detection system,
    driver assistance system,
  ]
---

> Citations: 1,513 | Paper Published: 23 Apr 2020 | Institutions: Academia Sinica | Authors: Alexey Bochkovskiy, Chien-Yao Wang, Hong-Yuan Mark Liao

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper discusses the use of various features to improve the accuracy of Convolutional Neural Networks (CNNs) on large datasets. The authors propose the use of new features and combinations of existing ones to achieve state-of-the-art results on the MS COCO dataset.

:::


## Contributions 

- Proposing the use of new features such as Weighted-Residual-Connections (WRC), Cross-Stage-Partial-connections (CSP), Cross mini-Batch Normalization (CmBN), Self-adversarial-training (SAT), Mish activation, Mosaic data augmentation, DropBlock regularization, and CIoU loss to improve the accuracy of CNNs on large datasets.
- Combining some of these new features with existing ones to achieve state-of-the-art results on the MS COCO dataset, with an average precision (AP) of 43.5% and an AP50 of 65.7% at a real-time speed of ~65 FPS on Tesla V100.

## Practical Implications

- The proposed features and combinations of existing ones can improve the accuracy of CNNs on large datasets.
- The state-of-the-art results achieved on the MS COCO dataset can be useful for various computer vision applications, such as object detection and segmentation.
- The source code provided by the authors can be used by researchers and practitioners to implement the proposed features and reproduce the results.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

- Proposing new features such as Weighted-Residual-Connections (WRC), Cross-Stage-Partial-connections (CSP), Cross mini-Batch Normalization (CmBN), Self-adversarial-training (SAT), Mish activation, Mosaic data augmentation, DropBlock regularization, and CIoU loss.
- Combining some of these new features with existing ones such as batch-normalization and residual-connections to improve the accuracy of CNNs on large datasets.
- Testing the proposed features and combinations of features on the MS COCO dataset for object detection and segmentation tasks.
- Evaluating the performance of the proposed models in terms of average precision (AP) and real-time speed on Tesla V100.

:::

## Data
The data used in this paper is the MS COCO dataset, which is a large-scale object detection, segmentation, and captioning dataset. It contains over 330K images with more than 2.5 million object instances labeled with 80 different categories.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

The paper achieved state-of-the-art results on the MS COCO dataset for object detection and segmentation tasks, with an average precision (AP) of 43.5% and an AP50 of 65.7% at a real-time speed of ~65 FPS on Tesla V100. These results were achieved using a combination of features, such as Weighted-Residual-Connections (WRC), Cross-Stage-Partial-connections (CSP), Cross mini-Batch Normalization (CmBN), Self-adversarial-training (SAT), Mish activation, Mosaic data augmentation, DropBlock regularization, and CIoU loss. The paper provides a detailed analysis of the impact of each proposed feature and combination of features on the performance of the models.

:::


## Limitations

- The proposed features and combinations of features may not be applicable to all types of CNN models, tasks, and datasets.
- The experiments were conducted on a single dataset, and the results may not generalize to other datasets or real-world scenarios.


