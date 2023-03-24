---
id: hyperspectral-image-classification
title: 'Deep Convolutional Neural Networks for Hyperspectral Image Classification'
sidebar_label: Hyperspectral Image Classification
keywords:
  [
    hyperspectral image classification,
    deep convolutional neural networks,
    spectral domain,
  ]
---

> Citations: 826 | Paper Published: 30 Jul 2015 | Institutions: Beijing University of Chemical Technology, Southwest Jiaotong University, University of Colorado Boulder | Authors: Wei Hu, Yangyu Huang, Li Wei, Fan Zhang, Heng-Chao Li, Heng-Chao Li

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper proposes the use of deep convolutional neural networks to classify hyperspectral images directly in spectral domain. The proposed method achieves better classification performance than traditional methods such as support vector machines and conventional deep learning-based methods.
:::


## Contributions 

The contribution of this paper is the proposal and demonstration of a simple but effective convolutional neural network architecture for hyperspectral image classification. The proposed method achieves better performance than traditional methods such as support vector machines and conventional deep learning-based methods, based on experimental results using several hyperspectral image datasets.

## Practical Implications

The practical implication of this paper is the development of a novel method for hyperspectral image classification using deep convolutional neural networks. This can have applications in various fields such as remote sensing, medical imaging, and surveillance systems where accurate identification and classification of objects or materials based on spectral information are important. The proposed method has shown better performance than traditional methods which could lead to more efficient and reliable analysis of hyperspectral data in these areas.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

The paper proposes the use of deep convolutional neural networks for hyperspectral image classification. The proposed classifier architecture contains five layers: input layer, convolutional layer, max pooling layer, full connection layer and output layer. These five layers are implemented on each spectral signature to discriminate against others. In addition, backpropagation is used in training the network by minimizing a cost function and computing partial derivatives with respect to trainable parameters using gradient descent method.

:::

## Data
The paper has used several hyperspectral image datasets for experimental evaluation of the proposed method. The specific details about these datasets are not mentioned in the abstract or context provided.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

- For one dataset called Pavia University scene with 9 classes, SVM had an overall classification rate of 91.5%, while the proposed CNN approach achieved a higher rate of 94%.
- For another dataset called Indian Pine with 16 classes, SVM had an overall classification rate of around 80%, whereas our proposed method obtained over ~85% for all cases except when using only two training samples per class where it was slightly lower at ~83%. 
- In general across multiple datasets tested by this study including Salinas Valley Scene data set which has more number(224 bands), Our model outperformed other models like Deep Belief Network(DBN).

:::


## Limitations

The limitations of this paper are not mentioned in the abstract or context provided. It is possible that the authors have discussed them in detail within the full text of their research article, which we do not have access to at present.


