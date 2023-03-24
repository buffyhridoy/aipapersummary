---
id: feature-pyramid-networks
title: 'Feature Pyramid Networks for Object Detection'
sidebar_label: Feature Pyramid Networks
keywords:
  [
    feature pyramid networks,
    object detection,
    object detection in cluttered scenes,
    Pyramid Networks,
    Pyramid Networks for Object Detection,
    adjacent regions,
    Real Time Object Detection,
  ]
---

> Citations: 7,876 | Paper Published: 21 Jul 2017 | Institutions: Cornell University, Facebook | Authors:Tsung-Yi Lin, Piotr Dollár, Ross Girshick, Kaiming He, Bharath Hariharan, Serge Belongie

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

This paper proposes a Feature Pyramid Network (FPN) that exploits the inherent multi-scale, pyramidal hierarchy of deep convolutional networks to construct feature pyramids with marginal extra cost. FPN shows significant improvement as a generic feature extractor in several applications and achieves state-of-the-art single-model results on the COCO detection benchmark without bells and whistles.

:::


## Contributions 

- Proposing a Feature Pyramid Network (FPN) that exploits the inherent multi-scale, pyramidal hierarchy of deep convolutional networks to construct feature pyramids with marginal extra cost.
- Developing a top-down architecture with lateral connections for building high-level semantic feature maps at all scales.
- Showing that FPN can be used as a generic feature extractor in several applications and achieves state-of-the-art single-model results on the COCO detection benchmark without bells and whistles.
- Providing a practical and accurate solution to multi-scale object detection that can run at 5 FPS on a GPU.

## Practical Implications

- The proposed Feature Pyramid Network (FPN) provides a practical and accurate solution to multi-scale object detection that can run at 5 FPS on a GPU.
- FPN can be used as a generic feature extractor in several applications, which can improve the performance of object detection systems.
- The study suggests that despite the strong representational power of deep ConvNets and their implicit robustness to scale variation, it is still critical to explicitly address multiscale problems using pyramid representations.
- The method presented in this paper can be used by researchers and practitioners to improve the performance of object detection systems without the need for computing image pyramids.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

The main method proposed in this paper is the Feature Pyramid Network (FPN), which is a top-down architecture with lateral connections that exploits the inherent multi-scale, pyramidal hierarchy of deep convolutional networks to construct feature pyramids with marginal extra cost. FPN is used as a generic feature extractor in several applications and achieves state-of-the-art single-model results on the COCO detection benchmark without bells and whistles.

:::

## Data
The paper uses the COCO (Common Objects in Context) dataset for evaluating the proposed method. The COCO dataset is a large-scale object detection, segmentation, and captioning dataset that contains over 330K images with more than 2.5 million object instances labeled with 80 different object categories.

## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

The paper reports state-of-the-art single-model results on the COCO detection benchmark without bells and whistles, surpassing all existing single-model entries including those from the COCO 2016 challenge winners. Using a basic Faster R-CNN system, the proposed method achieves an Average Precision (AP) of 36.2% on the COCO test-dev set, which is a significant improvement over the previous state-of-the-art result of 34.4%. The proposed method also achieves better results on small, medium, and large objects compared to the previous state-of-the-art methods. The method can run at 5 FPS on a GPU, making it a practical and accurate solution to multi-scale object detection.

:::


## Limitations

The paper does not mention any significant limitations of the proposed method. However, it suggests that a stronger architecture of the head may improve upon the results, which is beyond the focus of this paper. The paper also mentions that they have experimented with more sophisticated blocks and observed marginally better results, but simplicity is central to their design, and they have found that their model is robust to many design choices.



