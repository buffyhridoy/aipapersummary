---
id: cascade-r-cnn
title: 'Cascade R-CNN: Delving Into High Quality Object Detection'
sidebar_label: Cascade R-CNN
keywords:
  [
    cascade rcnn,
    object detection,
    object detection in cluttered scenes,
    multiscale intensity differences,
    adjacent regions,
    High Quality Object Detection,
  ]
---

> Citations: 1,608 | Paper Published: 18 Jun 2018 | Institutions: University of California, San Diego | Authors: Zhaowei Cai, Nuno Vasconcelos

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

This paper proposes a multi-stage object detection architecture called Cascade R-CNN to address the problem of overfitting and inference-time mismatch in object detection. It consists of a sequence of detectors trained with increasing IoU thresholds to be sequentially more selective against close false positives.

:::


## Contributions 

- Proposing a new object detection architecture called Cascade R-CNN that addresses the problems of overfitting during training and inference-time mismatch between IoUs.
- Showing that the Cascade R-CNN outperforms all single-model object detectors on the COCO dataset and is widely applicable across detector architectures.

## Practical Implications

- The proposed Cascade R-CNN architecture can be used to improve the performance of object detection systems in various applications, such as autonomous driving, surveillance, and robotics.
- The Cascade R-CNN can be applied to different detector architectures, making it a versatile and widely applicable approach.
- The paper highlights the importance of addressing the problems of overfitting and inference-time mismatch in object detection, which can lead to more accurate and reliable detection systems.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

- Proposing a new object detection architecture called Cascade R-CNN that consists of a sequence of detectors trained with increasing IoU thresholds.
- Training the detectors stage by stage, leveraging the observation that the output of a detector is a good distribution for training the next higher quality detector.
- Applying the same cascade procedure at inference to enable a closer match between the hypotheses and the detector quality of each stage.

:::

## Data
The authors have used the COCO dataset for evaluating the performance of the proposed Cascade R-CNN architecture. The COCO dataset is a widely used benchmark for object detection, segmentation, and captioning tasks. It contains a large number of images with complex scenes and a diverse set of object categories, making it a challenging dataset for object detection. 

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

- Cascade R-CNN with ResNet-50 backbone: achieves an AP of 42.8% at an IoU threshold of 0.5, and an AP of 23.7% at an IoU threshold of 0.9.
- Cascade R-CNN with ResNet-101 backbone: achieves an AP of 44.2% at an IoU threshold of 0.5, and an AP of 25.1% at an IoU threshold of 0.9.

:::


## Limitations

The limitations of this paper are not explicitly mentioned. However, one potential limitation could be that the proposed Cascade R-CNN architecture may require more computational resources and longer training time compared to single-model object detectors, due to the use of multiple stages of detectors with increasing IoU thresholds. Another limitation could be that the performance gains of the Cascade R-CNN may saturate or even degrade when applied to datasets with different characteristics or in different application domains.


