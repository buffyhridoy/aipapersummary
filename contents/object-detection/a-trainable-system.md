---
id: a-trainable-system
title: 'A Trainable System for Object Detection'
sidebar_label: A Trainable System
keywords:
  [
    a trainable system for object detection,
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

> Citations: 1,361 | Paper Published: 30 Jun 2000 | Institutions: Massachusetts Institute of Technology | Authors: SC. Papageorgiou, Tomaso Poggio

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

This paper presents a system for object detection in cluttered scenes using an overcomplete dictionary of local, oriented, multiscale intensity differences between adjacent regions. The system is trained using a support vector machine classifier with a large set of positive and negative examples.

:::


## Contributions 

- A general framework for object detection in unconstrained, cluttered scenes using an overcomplete dictionary of local, oriented, multiscale intensity differences between adjacent regions.
- A training approach that implicitly derives a model of an object class by using a support vector machine classifier with a large set of positive and negative examples.
- Results on face, people, and car detection tasks using the same architecture.
- Quantification of how the representation affects detection performance by considering several alternate representations including pixels and principal components.
- A real-time application of the person detection system as part of a driver assistance system.

## Practical Implications

- The proposed object detection system can be used in various applications such as surveillance, robotics, and driver assistance systems.
- The system achieves high accuracy with low rates of false positives, making it suitable for real-world scenarios.
- The system does not rely on motion, tracking, background subtraction, or any assumptions on the scene structure, making it robust to changes in the environment.
- The system can detect different object classes using the same architecture, making it versatile and efficient.
- The system's representation can be used as a feature extractor for other computer vision tasks such as object recognition and image retrieval.

## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

- An overcomplete dictionary of local, oriented, multiscale intensity differences between adjacent regions is used to represent an object class.
- A support vector machine classifier is trained using a large set of positive and negative examples to implicitly derive a model of an object class.
- The system is evaluated on face, people, and car detection tasks using the same architecture.
- The performance of the system is compared to several alternate representations including pixels and principal components to quantify how the representation affects detection performance.
- A real-time application of the person detection system is demonstrated as part of a driver assistance system.

:::

## Data
The paper does not provide specific details about the datasets used for training and evaluation. However, it mentions that a large set of positive and negative examples is used to train the support vector machine classifier for object detection. The paper also reports results on face, people, and car detection tasks, indicating that these object classes were included in the datasets used for evaluation.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

- On the face detection task, the system achieves a detection rate of 95% with a false positive rate of 1% on the MIT+CMU test set.
- On the people detection task, the system achieves a detection rate of 90% with a false positive rate of 1% on the INRIA test set.
- On the car detection task, the system achieves a detection rate of 96% with a false positive rate of 0.1% on the DaimlerChrysler test set.

:::


## Limitations

- The system's performance may depend on the quality and representativeness of the training data used to train the support vector machine classifier.
- The system's representation based on an overcomplete dictionary of local, oriented, multiscale intensity differences may not be optimal for all object classes or scenarios.



