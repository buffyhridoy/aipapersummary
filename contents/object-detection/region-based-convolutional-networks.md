---
id: region-based-convolutional-networks
title: 'Region-Based Convolutional Networks for Accurate Object Detection and Segmentation'
sidebar_label: Region-Based Convolutional Networks
keywords:
  [
    region based convolutional networks,
    object detection,
    object detection in cluttered scenes,
    Region based Convolutional Networks,
    Region based Convolutional Networks for Object Detection,
    adjacent regions,
    Real Time Object Detection,
  ]
---

> Citations: 1,514 | Paper Published: 01 Jan 2016 | Institutions: Microsoft, University of California, Berkeley | Authors: Ross Girshick, Jeff Donahue, Trevor Darrell, Jitendra Malik

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper proposes a simple and scalable object detection algorithm that combines high-capacity convolutional networks with bottom-up region proposals to achieve better performance on the PASCAL VOC object detection task. The proposed model is called R-CNN or Region-based Convolutional Network.

:::


## Contributions 

- Proposing a simple and scalable object detection algorithm that combines high-capacity convolutional networks with bottom-up region proposals to achieve better performance on the PASCAL VOC object detection task.
- Introducing the concept of supervised pre-training for an auxiliary task, followed by domain-specific fine-tuning, to boost performance significantly when labeled training data are scarce.
- Providing a new state-of-the-art performance on the PASCAL VOC 2012 object detection task with a mean average precision (mAP) of 62.4 percent.


## Practical Implications

- The proposed R-CNN model can be used for object detection tasks in various applications such as autonomous driving, surveillance, and robotics.
- The supervised pre-training approach can be used to improve the performance of object detection models when labeled training data are scarce.
- The proposed algorithm can be used as a baseline for future research in object detection and related fields.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

- The proposed R-CNN model combines high-capacity convolutional networks with bottom-up region proposals to achieve better performance on the PASCAL VOC object detection task.
- The model is trained in two stages: (1) pre-training on a large dataset for an auxiliary task, and (2) fine-tuning on the target object detection dataset.
- The selective search algorithm is used to generate region proposals for the object detection task.
- The model is trained using a multi-task loss function that combines classification and bounding box regression losses.

:::

## Data
The paper has used the PASCAL VOC 2012 object detection dataset to evaluate the proposed R-CNN model. Additionally, the paper has also presented results on the ILSVRC2013 detection dataset.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

- The proposed R-CNN model achieved a mean average precision (mAP) of 62.4%.
- The R-CNN model outperformed four strong baselines, including SegDPM.
- The paper also reports results on the ILSVRC2013 detection dataset, where the R-CNN model achieved a mAP of 31.4%. 

:::


## Limitations

- The R-CNN model is computationally expensive and slow at test time, as it requires running a CNN on each region proposal. This limits its practical use in real-time applications.
- The model requires a large amount of GPU memory during training, which can be a bottleneck for some users.



