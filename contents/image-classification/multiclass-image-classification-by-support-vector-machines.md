---
id: multiclass-image-classification-by-support-vector-machines
title: 'A Relative Evaluation of Multiclass Image Classification by Support Vector Machines'
sidebar_label: Multiclass Image Classification by Support Vector Machines
keywords:
  [
    multiclass image classification,
    support vector machines,
    svm,
    remotely sensed data,
    multiclass classification,
    ensemble based approaches,
    remotely sensed data analysis,
    airborne sensor data,
  ]
---

> Citations: 880 | Paper Published: 14 Jun 2004 | Institutions: University of Southampton | Authors: Giles M. Foody, Ajay Mathur

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper evaluates the potential of support vector machines (SVMs) as classifiers for remotely sensed data, particularly in multiclass classification. The study compares SVM with other popular classifiers and examines the effect of training set size on accuracy.

:::


## Contributions 

The contribution of this paper is to evaluate the potential of support vector machines (SVMs) as classifiers for remotely sensed data, particularly in multiclass classification. The study compares SVM with other popular classifiers and examines the effect of training set size on accuracy.

## Practical Implications

The practical implications of this paper are that it provides evidence for the effectiveness of SVMs as classifiers in remote sensing applications, particularly in multiclass classification. The study also highlights the importance of training set size on accuracy and suggests that larger training sets generally lead to more accurate classifications across all techniques tested. Additionally, while SVM was found to be the most accurate classifier overall, other methods may still have value when used together with ensemble-based approaches. Overall, these findings can inform decision-making processes related to remotely sensed data analysis and improve our ability to accurately classify different land cover types from airborne sensor data.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

The methods used in this paper involved acquiring imagery from an airborne thematic mapper (ATM) and using it to train and test different classifiers for multiclass classification of remotely sensed data. The study compared the accuracy of support vector machines (SVMs), discriminant analysis, decision trees, and multilayer perceptron neural networks across a range of training set sizes. To ensure robustness in results, five independent samples were derived from each available training dataset size except when all 100 pixels per class were used as one sample. Accuracy was assessed using an additional random testing set consisting of 320 pixels that was acquired independently for use with all classifications tested. Finally, statistical analyses were conducted to compare the performance differences between these techniques while accounting for related nature among samples within each technique's output predictions or labels assigned by them during evaluation against ground truth information provided through manual interpretation or other means such as field surveys etc..

:::

## Data
The data used in this paper is imagery acquired by an airborne thematic mapper (ATM). The dataset was classified using a series of classifiers, including support vector machines (SVM), discriminant analysis, decision tree and multilayer perceptron neural network. For each size of training set, five independent samples were derived from the available training data to avoid extreme results. Accuracy was assessed using a further independent random sample of 320 pixels that were acquired for use as testing sets across all classification analyses undertaken.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

The study found that the SVM approach was generally more accurate than other classifiers tested, with an accuracy of 93.75% obtained from the SVM trained with 100 cases of each class. This classification was significantly more accurate than those derived from decision tree and discriminant analysis methods (p<0.05). The value of γ parameter had a marked impact on classification accuracy, ranging between 0.005 to 0.08 in this study's classifications using SVMs; while number support vectors used ranged from 74 to331 across all analyses undertaken for different training set sizes.

:::


## Limitations

- It only evaluated a limited number of classifiers for multiclass classification, and there may be other methods or combinations thereof that could yield even better results. 
- The study focused solely on airborne sensor data and did not examine how these techniques might perform with different types of remotely sensed imagery (e.g., satellite-based).


