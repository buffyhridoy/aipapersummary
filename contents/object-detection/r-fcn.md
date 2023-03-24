---
id: r-fcn
title: 'R-FCN: Object Detection via Region-based Fully Convolutional Networks'
sidebar_label: R-FCN
keywords:
  [
    region based fully convolutional networks,
    object detection,
    object detection in cluttered scenes,
    Region based Fully Convolutional Networks,
    Region based Fully Convolutional Networks for Object Detection,
    adjacent regions,
    Real Time Object Detection,
  ]
---


> Citations: 3,791 | Paper Published: 20 May 2016 | Institutions: Microsoft, Tsinghua University, Xi'an Jiaotong University | Authors: Jifeng Dai, Yi Li, Kaiming He, Jian Sun

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper presents a region-based, fully convolutional network for object detection that uses position-sensitive score maps to address the dilemma between translation-invariance in image classification and translation-variance in object detection. The proposed method achieves competitive results on the PASCAL VOC datasets with a test-time speed of 170ms per image.

:::


## Contributions 

- The proposal of a region-based, fully convolutional network for object detection that is more accurate and efficient than previous methods.
- The introduction of position-sensitive score maps to address the dilemma between translation-invariance in image classification and translation-variance in object detection.
- The ability to adopt fully convolutional image classifier backbones, such as the latest Residual Networks (ResNets), for object detection.
- Competitive results on the PASCAL VOC datasets with a test-time speed of 170ms per image. 


## Practical Implications

- The proposed region-based, fully convolutional network for object detection can be used in real-world applications that require accurate and efficient object detection.
- The method can be used with state-of-the-art image classification backbones, such as ResNets, which are fully convolutional by design.
- The method achieves competitive results on the PASCAL VOC datasets, which are widely used in the computer vision community.
- The method is faster than previous region-based detectors during both training and inference, making it more practical for real-world applications.
- The code for the proposed method is publicly available, making it easier for researchers and practitioners to use and build upon.

## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

- Region-based, fully convolutional network for object detection.
- Position-sensitive score maps to address the dilemma between translation-invariance in image classification and translation-variance in object detection.
- Use of fully convolutional image classifier backbones, such as the latest Residual Networks (ResNets), for object detection.
- Training and evaluation on the PASCAL VOC datasets.
- Comparison with previous state-of-the-art object detection methods, such as Fast/Faster R-CNN.

:::

## Data
The authors of the paper have used the PASCAL VOC datasets for training and evaluation of their proposed method. The PASCAL VOC datasets are widely used in the computer vision community for object detection tasks.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

- The proposed method achieves 83.6% mAP on the 2007 set of the PASCAL VOC dataset using the 101-layer ResNet.
- The test-time speed of the proposed method is 170ms per image, which is 2.5-20 times faster than the Faster R-CNN counterpart.
- The class-specific RPN has an mAP of 67.6%, which is about 9 points lower than the standard Faster R-CNN's 76.4%.

:::


## Limitations

The paper does not explicitly mention any limitations of their proposed method. However, one potential limitation could be that the proposed method may not perform as well on datasets with more complex and diverse object categories than the PASCAL VOC dataset. Additionally, the proposed method may require more computational resources during training than some other object detection methods due to the use of position-sensitive score maps.



