---
id: faster-r-cnn
title: 'Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks'
sidebar_label: Faster R-CNN
keywords:
  [
    faster rcnn,
    object detection,
    object detection in cluttered scenes,
    Real Time Object Detection,
    Region Proposal Networks,
    Towards Real Time Object Detection,
    adjacent regions,
    Real Time Object Detection,
  ]
---

> Citations: 23,121 | Paper Published: 04 Jun 2015 | Institutions: University of Science and Technology of China, Microsoft, Facebook | Authors: Shaoqing Ren, Kaiming He, Ross Girshick, Jian Sun

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper introduces a Region Proposal Network (RPN) that generates high-quality region proposals for object detection. The RPN shares full-image convolutional features with the detection network, enabling nearly cost-free region proposals and achieving state-of-the-art accuracy on various datasets.

:::


## Contributions 

- Introducing a Region Proposal Network (RPN) that shares full-image convolutional features with the detection network, enabling nearly cost-free region proposals.
- Merging RPN and Fast R-CNN into a single network by sharing their convolutional features to achieve state-of-the-art object detection accuracy on various datasets.

## Practical Implications

The practical implications of this paper are that it introduces an efficient method for generating high-quality region proposals using a fully convolutional neural network called Region Proposal Network (RPN). This can be used in conjunction with other networks like Fast R-CNN to achieve state-of-the-art object detection accuracy on various datasets.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

- Introducing a Region Proposal Network (RPN) that shares full-image convolutional features with the detection network, enabling nearly cost-free region proposals.
- Training RPN end-to-end to generate high-quality region proposals simultaneously predicting object bounds and scores at each position.
- Merging RPN and Fast R-CNN into a single network by sharing their convolutional features.

:::

## Data
The paper has used various datasets for evaluating the proposed method, including PASCAL VOC 2007 and 2012, MS COCO, ILSVRC and COCO 2015.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

The paper proposes a Region Proposal Network (RPN) that shares full-image convolutional features with the detection network, enabling nearly cost-free region proposals. The RPN is a fully convolutional network that simultaneously predicts object bounds and objectness scores at each position. The RPN is trained end-to-end to generate high-quality region proposals, which are used by Fast R-CNN for detection. The proposed method achieved state-of-the-art object detection accuracy on various datasets such as PASCAL VOC 2007, 2012 and MS COCO with only 300 proposals per image. For very deep VGG-16 model, the detection system has a frame rate of 5fps (including all steps) on GPU. Faster R-CNN and RPN were used in several tracks for ILSVRC and COCO competitions where they formed foundations for first-place winning entries.

:::


## Limitations

- The proposed visualization techniques rely on computing the gradient of class scores with respect to input images, which may not always be feasible or effective for certain types of data.
- While qualitative analysis is provided in the study, there is no quantitative evaluation or comparison against other state-of-the-art methods that could provide a more comprehensive assessment of performance and effectiveness.
- It remains unclear how well these visualization techniques generalize across different datasets and tasks beyond those used in this particular study.



