---
id: multi-column-deep-neural-networks
title: 'Multi-column Deep Neural Networks for Image Classification'
sidebar_label: Multi-column Deep Neural Networks
keywords:
    [
        multi-column deep neural networks,
        multi-column deep neural networks for image classification,
        multi-column deep neural networks for image recognition,
        multi-column deep neural networks for handwritten digit classification,
        multi-column deep neural networks for traffic sign detection,
        multi-column deep neural networks for traffic sign recognition,
    ]
---

> Citations: 3,248 | Paper Published: 16 Jun 2012 | Institutions: Dalle Molle Institute for Artificial Intelligence Research | Authors: Dan Ciresan, Ueli Meier, Jürgen Schmidhuber

<!-- Prettier doesn't change this -->

:::tip Abstract in 2 Lines

The paper discusses the use of biologically plausible, wide and deep artificial neural network architectures to achieve human-like performance on tasks such as recognition of handwritten digits or traffic signs. The method outperforms traditional computer vision and machine learning methods in various image classification benchmarks.

:::

## Contributions

The paper presents a method for training wide and deep convolutional neural networks (DNN) using simple online back-propagation. The trained DNNs achieve greatly improved records on various image classification benchmarks, including MNIST, Latin letters, Chinese characters, traffic signs, NORB (jittered cluttered), and CIFAR10. The authors demonstrate that unsupervised initialization/pretraining is not necessary for achieving high performance with their approach but combining several DNN columns into a Multi-column DNN further decreases the error rate by 30-40%.

## Practical Implications

The practical implications of this paper are that the proposed method can be used to improve image recognition systems in various applications, such as self-driving cars and handwriting recognition. The approach achieves human-like performance on tasks like traffic sign detection and handwritten digit classification without requiring unsupervised pre-training or additional unlabeled data sources. This makes it a promising technique for improving computer vision algorithms in real-world scenarios where labeled training data is available but large amounts of unlabeled data may not be accessible.

## Methods

<!-- Prettier doesn't change this -->

:::info Methodology

The paper uses a wide and deep convolutional neural network (DNN) architecture that combines several techniques in a novel way. The DNNs have hundreds of maps per layer, are inspired by the Neocognitron with many layers stacked on top of each other comparable to those found between retina and visual cortex of macaque monkeys. Simple online back-propagation is used for training without requiring unsupervised pre-training or additional unlabeled data sources. Several DNN columns become experts on inputs preprocessed in different ways; their predictions are averaged to improve performance further. Graphics cards allow fast training using massively parallel processing units (GPUs).

:::

## Data

The paper uses various image classification benchmarks, including MNIST (handwritten digits), NIST SD 19 (digits and uppercase letters), Chinese characters, traffic signs, CIFAR10 (small images of objects in different categories) and NORB dataset with jittered clutter. The authors demonstrate that their approach achieves state-of-the-art performance on these datasets without requiring unsupervised pre-training or additional unlabeled data sources.

## Results

<!-- Prettier doesn't change this -->

:::note Performance Analysis

- On MNIST dataset, they achieved an error rate of 0.23%, which is a significant improvement over previous methods.
- For traffic sign recognition benchmark, their approach outperformed humans by a factor of two with an overall accuracy score around 99%.
- They also report improvements ranging from around ~30%-~80%, depending upon specific datasets used for evaluation purposes.

:::

## Limitations

- One limitation of this paper is that the proposed method may not be suitable for all types of image recognition tasks. The authors mainly focus on classification benchmarks, and it remains to be seen how well their approach would perform in other applications such as object detection or semantic segmentation.

- Another potential limitation is that the DNN architecture used in this paper requires a large number of parameters, which can make training slow and computationally expensive. While graphics cards allow fast training using massively parallel processing units (GPUs), some researchers might find these requirements prohibitive.
