---
id: gan
title: 'Generative Adversarial Nets'
sidebar_label: GAN
keywords:
  [
    generative adversarial nets,
    generative adversarial networks,
    gan,
    gan for image tagging,
    gan for image synthesis,
    gan for image editing,
    gan for image generation,
    gan for image captioning,
    gan for image translation,
    gan for image super-resolution,
    gan for image inpainting,
  ]
---

> Citations: 29,410 | Paper Published: 08 Dec 2014 | Institutions: Université de Montréal, Indian Institute of Technology Delhi | Authors: Ian Goodfellow, Jean Pouget-Abadie, Mehdi Mirza, Bing Xu

<!-- Prettier doesn't change this -->

:::tip Abstract in 2 Lines

The paper proposes a new framework for training generative models using an adversarial process. This framework involves training two models simultaneously: a generative model and a discriminative model, with the aim of making the generated samples indistinguishable from the real ones.

:::


## Contributions

- Proposing a new framework for training generative models using an adversarial process.
- Demonstrating the potential of this framework through qualitative and quantitative evaluation of the generated samples.
- Exploring the special case when the generative model generates samples by passing random noise through a multilayer perceptron, and the discriminative model is also a multilayer perceptron, and showing that both models can be trained using only backpropagation and dropout algorithms.


## Practical Implications

- The proposed framework can be used to generate high-quality samples that are indistinguishable from real data, which can be useful in various applications such as image and speech synthesis, data augmentation, and anomaly detection.
- The framework is easy to implement and does not require any Markov chains or unrolled approximate inference networks, which makes it computationally efficient and scalable.
- The paper demonstrates the viability of the adversarial modeling framework, which suggests that this approach could be useful in other research directions as well.


## Methods

<!-- Prettier doesn't change this -->

:::info Methodology

The paper proposes a new framework for training generative models using an adversarial process. The framework involves training two models simultaneously: a generative model and a discriminative model, with the aim of making the generated samples indistinguishable from the real ones. The authors demonstrate the viability of this framework through qualitative and quantitative evaluation of the generated samples. The authors also explore the special case when the generative model generates samples by passing random noise through a multilayer perceptron, and the discriminative model is also a multilayer perceptron, and show that both models can be trained using only backpropagation and dropout algorithms.

:::


## Data

The paper does not mention any specific dataset used in the experiments. However, it mentions that the proposed framework can be applied to various types of data, including images, speech, and text.


## Results

<!-- Prettier doesn't change this -->

:::note Performance Analysis

- Inception score: a metric that measures the quality and diversity of the generated samples. The proposed framework achieves an inception score that is competitive with state-of-the-art generative models.
- Frechet distance: a metric that measures the similarity between the distribution of the generated samples and the distribution of the real data. The proposed framework achieves a Frechet distance that is lower than that of other generative models.
- Nearest neighbor classification: a metric that measures the quality of the learned representations. The proposed framework achieves a classification accuracy that is competitive with other generative models.

:::


## Limitations

- The proposed framework may suffer from mode collapse, where the generator learns to produce only a limited set of samples that are similar to each other, rather than the full diversity of the real data.
- The paper also does not address the issue of evaluating the quality of the generated samples in a more objective and quantitative manner, such as through user studies or real-world applications.
