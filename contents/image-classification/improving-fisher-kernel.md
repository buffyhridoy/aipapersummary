---
id: improving-fisher-kernel
title: 'Improving The Fisher Kernel for Large-scale Image Classification'
sidebar_label: Improving The Fisher Kernel
keywords:
    [
    fisher kernel,
    fisher kernel for large scale image classification,
    fisher kernel for image classification,
    improving fisher kernel,
    improving the fisher kernel,
    ]
---

> Citations: 2,799 | Paper Published: 05 Sep 2010 | Institutions: Xerox | Authors: Florent Perronnin, Jorge Sanchez, Thomas Mensink

<!-- Prettier doesn't change this -->

:::tip Abstract in 2 Lines

The paper introduces the Fisher Kernel (FK) framework for image classification, which combines generative and discriminative approaches. The authors show that with modifications to the original FK framework, they can improve accuracy on several datasets compared to traditional bag-of-visual-words representations.

:::

## Contributions

- The first part shows that with modifications to the Fisher Kernel (FK) framework, accuracy in image classification can be boosted beyond what is achieved by the popular bag-of-visual-words (BOV) representation.
- In the second part, an evaluation involving hundreds of thousands of training images compares classifiers learned on Flickr groups and ImageNet datasets for learning image classifiers on large annotated datasets.

## Practical Implications

- The proposed improved Fisher vector has the potential to become a new standard representation in image classification, as it achieves state-of-the-art results on several datasets using only SIFT features and costless linear classifiers.
- Flickr groups can be used as an abundant resource for training material for learning image classifiers, complementing more carefully annotated datasets like ImageNet.

## Methods

<!-- Prettier doesn't change this -->

:::info Methodology

The paper introduces the Fisher Kernel (FK) framework for image classification, which combines generative and discriminative approaches. The authors modify this framework to improve accuracy in image classification beyond what is achieved by traditional bag-of-visual-words representations. They evaluate their approach on several datasets using SIFT features and costless linear classifiers. Additionally, they compare classifiers learned from Flickr groups with those learned from ImageNet dataset as an application of their proposed method.

:::

## The Fisher Vector

- The gradient of the log-likelihood describes the contribution of the parameters to the generation process.
- The authors underline that learning a kernel classifier using the kernel is equivalent to learning a linear classifier on the Fisher vectors GXλ .
- The authors denote λ = {wi, µi, Σi, i = 1 . . .K} where wi, µi and Σi are respectively the mixture weight, mean vector and covariance matrix of Gaussian ui.
- Let D denote the dimensionality of the descriptors xt.
- The final gradient vector GXλ is the concatenation of the GXµ,i and GXσ,i vectors for i = 1 . . .K and is therefore 2KD-dimensional.

## L2 normalization

- The authors note that the signature still depends on the proportion of image-specific information ω.
- Especially, small objects with a small ω value will be difficult to detect.
- This is not to say that the L2 norm of the Fisher vector is not discriminative.
- In practice, removing the dependence on the L2 norm (i.e. on both ω and ||∇λEx∼q log uλ(x)||) can lead to large improvements.

## Power normalization

- The second improvement is motivated by an empirical observation: as the number of Gaussians increases, Fisher vectors become sparser.
- Hence, as the number of Gaussians increases, the distribution of features in a given dimension becomes more peaky around zero.
- Since the dot-product / L2 distance are poor measures of similarity on sparse vectors, the authors are left with two choices: – We can replace the dot-product by a kernel which is more robust on sparse vectors.
- In all their experiments, the authors set K = 256 as it provides a good compromise between computational cost and classification accuracy. When combining the power and the L2 normalizations, the authors apply the power normalization first and then the L2 normalization.

## Data

The paper uses two datasets for evaluation: PASCAL VOC 2007 and CalTech 256. Additionally, the authors compare classifiers learned from Flickr groups with those learned from ImageNet dataset as an application of their proposed method.

## Results

<!-- Prettier doesn't change this -->

:::note Performance Analysis

- On PASCAL VOC 2007 dataset, they increase Average Precision (AP) from 47.9% to 58.3%, achieving state-of-the-art performance.
- Similarly, on CalTech256 dataset also they achieve state of art result.
- They compare classifiers learned from Flickr groups with those learned from ImageNet dataset as an application of their proposed method involving hundreds of thousands training images showing promising results for learning image classifiers at a larger scale complementing more carefully annotated datasets like ImageNet.

:::

## Limitations

- The proposed modifications and results are specific to image classification tasks using SIFT descriptors and linear classifiers.
- Performance of this method may vary for other types of data or with different feature extraction methods/classifiers.
- Further research would be required before drawing definitive conclusions about its effectiveness compared to traditional sources such as ImageNet which has been widely used by researchers over many years now.
- Although their modified FK framework improves accuracy beyond what can be achieved through bag-of-visual-word representations alone, there still remains scope for improving upon these techniques even further especially given recent advances made in deep neural networks etc..
