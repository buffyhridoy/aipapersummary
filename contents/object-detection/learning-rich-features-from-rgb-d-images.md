---
id: learning-rich-features-from-rgb-d-images
title: 'Learning Rich Features from RGB-D Images for Object Detection and Segmentation'
sidebar_label: Learning Rich Features from RGB-D Images
keywords:
  [
    learning rich features from rgbd images,
    rich features from rgb d images,
    rgbd images,
    object detection,
    object detection system,
  ]
---

> Citations: 1,226 | Paper Published: 06 Sep 2014 | Institutions: University of California1, University of Los Andes | Authors: Saurabh Gupta, Ross Girshick, Pablo Arbeláez, Pablo Arbeláez, Jitendra Malik

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

This paper proposes a new approach for object detection and instance segmentation in RGB-D images using semantically rich image and depth features. The proposed method achieves a 56% relative improvement over existing methods for object detection and a 24% relative improvement over current state-of-the-art for semantic scene segmentation.

:::


## Contributions 

- Proposing a new geocentric embedding for depth images that encodes height above ground and angle with gravity for each pixel in addition to the horizontal disparity, which works better than using raw depth images for learning feature representations with convolutional neural networks.
- Developing an object detection system that achieves a 56% relative improvement over existing methods.
- Proposing a decision forest approach for instance segmentation that classifies pixels in the detection window as foreground or background using a family of unary and binary tests that query shape and geocentric pose features.
- Improving semantic segmentation performance by using object detections to compute additional features for superpixels in the semantic segmentation system.

## Practical Implications


- The proposed geocentric embedding for depth images can be used to improve the performance of object detection and instance segmentation in RGB-D images, which can be useful in various applications such as robotics, autonomous driving, and surveillance.
- The proposed object detection system can be used to detect objects in RGB-D images with higher accuracy than existing methods, which can be useful in applications such as object recognition, tracking, and scene understanding.
- The proposed decision forest approach for instance segmentation can be used to label pixels belonging to object instances found by the detector, which can be useful in applications such as object segmentation, tracking, and recognition.
- The proposed method for semantic segmentation can be used to improve the performance of existing semantic segmentation systems, which can be useful in applications such as scene understanding, image and video analysis, and robotics.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

- Geocentric Embedding for Depth Images: A new geocentric embedding for depth images is proposed that encodes height above ground and angle with gravity for each pixel in addition to the horizontal disparity. This embedding is used to learn feature representations with convolutional neural networks for object detection and instance segmentation.
- Object Detection: A two-stage object detection system is developed that first generates object proposals using selective search and then classifies the proposals using a convolutional neural network. The proposed geocentric embedding is used to learn feature representations for object detection.
- Instance Segmentation: A decision forest approach is proposed for instance segmentation that classifies pixels in the detection window as foreground or background using a family of unary and binary tests that query shape and geocentric pose features.
- Semantic Segmentation: The output from the object detectors is used in an existing superpixel classification framework for semantic scene segmentation. The proposed geocentric embedding is used to compute additional features for superpixels in the semantic segmentation system.

:::

## Data
The paper uses the NYU Depth v2 dataset, which consists of RGB-D images of indoor scenes. The dataset contains 1449 densely labeled pairs of aligned RGB and depth images, with 795 for training and 654 for testing. The dataset includes 13 object categories, including bed, books, ceiling, chair, floor, furniture, objects, picture, sofa, table, TV, wall, and window. The proposed methods are evaluated on this dataset for object detection, instance segmentation, and semantic segmentation tasks.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

- Object Detection: The proposed object detection system achieves an average precision of 37.3%, which is a 56% relative improvement over existing methods.
- Instance Segmentation: The proposed decision forest approach for instance segmentation achieves an average precision of 28.5%, which is a 50% relative improvement over existing methods.
- Semantic Segmentation: The proposed method for semantic segmentation achieves a 24% relative improvement over current state-of-the-art for the object categories that were studied.

:::


## Limitations

- The proposed methods are limited to the object categories included in the NYU Depth v2 dataset, and the performance on other object categories is not evaluated.
- The proposed methods require a large amount of training data, which may not be available in some applications.



