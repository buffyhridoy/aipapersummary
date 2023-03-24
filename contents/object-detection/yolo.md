---
id: yolo
title: 'You Only Look Once: Unified, Real-Time Object Detection'
sidebar_label: YOLO
keywords:
    [
        You Only Look Once,
        Detection,
        Unified, Real-Time Object Detection,
        yolo
    ]
---

> Citations: 15,184 | Paper Published: 27 Jun 2016 | Institutions: University of Washington, Allen Institute for Artificial Intelligence, Facebook | Authors: Joseph Redmon, Santosh K. Divvala, Ross Girshick, Ali Farhadi

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper presents a new approach to object detection called YOLO, which frames the problem as a regression task and uses a single neural network for end-to-end optimization. The proposed architecture is extremely fast and outperforms other state-of-the-art methods in generalizing from natural images to artwork.

:::


## Contributions 

The contribution of this paper is the introduction of a new approach to object detection called YOLO, which frames the problem as a regression task and uses a single neural network for end-to-end optimization. The proposed architecture is extremely fast and outperforms other state-of-the-art methods in generalizing from natural images to artwork. Additionally, the paper examines tradeoffs between localization errors and false positives on background in experiments with different models.

## Practical Implications

The practical implications of this paper are that YOLO provides a simple and fast solution for object detection, making it ideal for applications that require real-time performance. The model can be trained directly on full images using a loss function that corresponds to detection performance, which simplifies the training process compared to classifier-based approaches. Additionally, YOLO generalizes well across different domains such as natural images and artwork, further increasing its applicability in various scenarios where robust object detection is required.




## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

The main method used in this paper is the YOLO (You Only Look Once) approach to object detection, which frames the problem as a regression task and uses a single neural network for end-to-end optimization. The model predicts bounding boxes and class probabilities directly from full images in one evaluation, making it extremely fast compared to other state-of-the-art methods. Additionally, experiments were conducted with different models that examined tradeoffs between localization errors and false positives on background. Finally, VGG-16 was also trained using YOLO but since it is slower than real-time only its accuracy was reported without further analysis of results due to speed limitations.

:::

## Data
The paper uses academic datasets for object detection to draw the training and testing data from the same distribution. Additionally, two other datasets were used: Picasso Dataset and People-Art Dataset, which are designed specifically for testing person detection on artwork. The authors also trained YOLO using VGG-16 architecture but only reported its accuracy without further analysis of results due to speed limitations compared with real-time performance achieved by YOLO model.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

The paper reports that YOLO achieves a mean average precision (mAP) of 57.9% on the VOC 2012 test set, which is lower than the current state-of-the-art but closer to original R-CNN using VGG-16 architecture. The system struggles with small objects compared to its closest competitors and scores around 8-10% lower in categories like bottle, sheep, and tv/monitor as compared to other methods such as R-CNN or Feature Edit. However, it performs better than others in some categories like cat and train where it achieved higher performance levels.

:::


## Limitations

- Strong spatial constraints on bounding box predictions: Since each grid cell only predicts two boxes and can only have one class, this limits the number of nearby objects that our model can predict. This makes it difficult for detecting small objects in groups such as flocks of birds.
- Difficulty generalizing to new or unusual aspect ratios or configurations: The model struggles with predicting bounding boxes for novel shapes since its training data is limited.



