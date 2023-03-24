---
id: fast-feature-pyramids
title: 'Fast Feature Pyramids for Object Detection'
sidebar_label: Fast Feature Pyramids
keywords:
  [
    fast feature pyramids,
    feature pyramids,
    fast feature pyramids for object detection,
    feature pyramids for object detection,
  ]
---

> Citations: 1,784  | Paper Published: 01 Aug 2014 | Institutions: Microsoft, California Institute of Technology, Cornell University | Authors: Piotr Dollár, Ron Appel, Serge Belongie, Pietro Perona

<!-- Prettier doesn't change this -->
:::tip Abstract in 2 Lines

The paper proposes a method to compute multi-resolution image features at a fraction of the cost, without sacrificing performance. This method yields considerable speedups with negligible loss in detection accuracy and is widely applicable to vision algorithms requiring fine-grained multi-scale analysis.

:::


## Contributions 

- The paper proposes a method to compute richer representations without paying a large computational price.
- The proposed method, called fast feature pyramids, is shown to be effective for pedestrian detection and general object detection using three distinct detection frameworks.

## Practical Implications

- The proposed fast feature pyramid method can significantly reduce the computational cost of object detection algorithms while maintaining high accuracy.
- This method can be applied to a wide range of vision algorithms that require multi-scale analysis, making it a valuable tool for computer vision researchers and practitioners.


## Methods
<!-- Prettier doesn't change this -->
:::info Methodology

The main method proposed in this paper is called "fast feature pyramids". This method involves computing finely sampled feature pyramids at octave-spaced scale intervals, which are then used to approximate features on a finely-sampled pyramid. This approximation is valid for images with broad spectra (most natural images) and fails for images with narrow band-pass spectra (e.g., periodic textures). The paper modifies three diverse visual recognition systems to use fast feature pyramids and shows results on both pedestrian detection and general object detection.

:::

## Data

- Caltech pedestrian dataset
- INRIA pedestrian dataset
- TUD-Brussels pedestrian dataset
- ETH pedestrian dataset
- PASCAL VOC object detection dataset


## Results
<!-- Prettier doesn't change this -->
:::note Performance Analysis

- On the Caltech pedestrian dataset, the proposed method achieves a miss rate of 13.6% at 10 fps, which is comparable to the state-of-the-art method ACF at 10 fps.
- On the INRIA pedestrian dataset, the proposed method achieves a miss rate of 8.8% at 10 fps, which is better than the state-of-the-art method ACF at 10 fps.
- On the TUD-Brussels pedestrian dataset, the proposed method achieves a miss rate of 8.5% at 10 fps, which is comparable to the state-of-the-art method ACF at 10 fps.
- On the ETH pedestrian dataset, the proposed method achieves a miss rate of 4.5% at 10 fps, which is better than the state-of-the-art method ACF at 10 fps.
- On the PASCAL VOC object detection dataset, the proposed method achieves a mean average precision (mAP) of 53.3%, which is comparable to the state-of-the-art method R-CNN.

:::


## Limitations

One limitation of this paper is that the proposed fast feature pyramid method may not work well for images with narrow band-pass spectra, such as periodic textures. This is because the approximation of features on a finely-sampled pyramid from octave-spaced scale intervals may not be accurate for such images. Another limitation is that the paper only evaluates the proposed method on pedestrian detection and general object detection tasks, and it is unclear how well the method would perform on other vision tasks.


