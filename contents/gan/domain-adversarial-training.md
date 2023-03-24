---
id: domain-adversarial-training
title: 'Domain-adversarial training of neural networks'
sidebar_label: Domain-adversarial Training
keywords:
    [
        domain-adversarial training,
        domain-adversarial training of neural networks,
        adversarial training,
        domain-adversarial neural network,
        dann,
    ]
---

> Citations: 4,760 | Paper Published: 01 Jan 2016 | Institutions: Skolkovo Institute of Science and Technology, Laval University, Université de Sherbrooke | Authors: Yaroslav Ganin, Evgeniya Ustinova, Hana Ajakan, Pascal Germain, Hugo Larochelle, François Laviolette, Mario Marchand, Victor Lempitsky

<!-- Prettier doesn't change this -->

:::tip Abstract in 2 Lines

This paper proposes a new approach for domain adaptation in which a neural network is trained on labeled data from the source domain and unlabeled data from the target domain. The approach promotes the emergence of features that are discriminative for the main learning task on the source domain and indiscriminate with respect to the shift between the domains.

:::

## Contributions

- Introducing a new approach for domain adaptation in which a neural network is trained on labeled data from the source domain and unlabeled data from the target domain.
- Proposing a domain-adversarial neural network (DANN) that uses standard layers and loss functions, and can be trained using standard backpropagation algorithms based on stochastic gradient descent or its modifications.
- Demonstrating the success of the proposed approach for two distinct classification problems (document sentiment analysis and image classification) and validating the approach for descriptor learning task in the context of person re-identification application.


## Practical Implications

- The proposed approach can be used to improve the performance of machine learning models in scenarios where the training and test data come from different distributions, which is a common problem in many real-world applications.
- The approach does not require labeled data from the target domain, which can be expensive or difficult to obtain in some cases.
- The proposed domain-adversarial neural network (DANN) is easy to implement using standard deep learning packages and can be trained using standard backpropagation algorithms, which makes it accessible to a wide range of researchers and practitioners.
- The success of the proposed approach for two distinct classification problems (document sentiment analysis and image classification) and validation for descriptor learning task in the context of person re-identification application suggests that it has the potential to be applied to other domains and tasks as well.

## Methods

<!-- Prettier doesn't change this -->

:::info Methodology

The paper proposes a domain-adversarial neural network (DANN) for domain adaptation, which is a modification of a standard neural network architecture that includes a gradient reversal layer. The DANN is trained on labeled data from the source domain and unlabeled data from the target domain, and it promotes the emergence of features that are discriminative for the main learning task on the source domain and indiscriminate with respect to the shift between the domains. The paper has demonstrated the success of the proposed approach for two distinct classification problems (document sentiment analysis and image classification) and validated the approach for descriptor learning task in the context of person re-identification application.

:::

## Data

The paper has used the Amazon reviews dataset, as pre-processed by Chen et al. (2012), which includes four domains, each one composed of reviews of a specific kind of product (books, dvd disks, electronics, and kitchen appliances). Reviews are encoded in 5 000 dimensional feature vectors of unigrams and bigrams, and labels are binary: "0" if the product is ranked up to 3 stars, and "1" if the product is ranked 4 or 5 stars. The paper has performed twelve domain adaptation tasks using this dataset.

## Results

<!-- Prettier doesn't change this -->

:::note Performance Analysis

- For document sentiment analysis, the paper has achieved an accuracy of 82.0% on the Amazon reviews dataset, which is a significant improvement over the previous state-of-the-art method that achieved an accuracy of 80.1%.
- For image classification, the paper has achieved an accuracy of 77.5% on the Office dataset, which is a significant improvement over the previous state-of-the-art method that achieved an accuracy of 68.4%.

:::

## Limitations

- The proposed approach assumes that the source and target domains are similar but different, and it may not work well in scenarios where the domains are very different.
- The paper has only evaluated the proposed approach on two distinct classification problems and one descriptor learning task, and it is unclear how well it would perform on other domains and tasks.
