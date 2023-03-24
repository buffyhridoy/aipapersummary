---
id: cycle-consistent-adversarial-networks
title: 'Unpaired Image-to-Image Translation Using Cycle-Consistent Adversarial Networks'
sidebar_label: Cycle-Consistent Adversarial Networks
keywords:
  [
    unpaired image-to-image translation,
    unpaired image-to-image translation using cycle-consistent adversarial networks,
    unpaired image-to-image translation using cycle-consistent adversarial networks for image synthesis,
    unpaired image-to-image translation using cycle-consistent adversarial networks for image editing,
    unpaired image-to-image translation using cycle-consistent adversarial networks for image generation,
    unpaired image-to-image translation using cycle-consistent adversarial networks for image captioning,
    unpaired image-to-image translation using cycle-consistent adversarial networks for image translation,
    unpaired image-to-image translation using cycle-consistent adversarial networks for image super-resolution,
    unpaired image-to-image translation using cycle-consistent adversarial networks for image inpainting,
    cycle-consistent adversarial networks,
    cycle-consistent adversarial networks for image synthesis,
    cycle-consistent adversarial networks for image editing,
    cycle-consistent adversarial networks for image generation,
    cycle-consistent adversarial networks for image captioning,
    cycle-consistent adversarial networks for image translation,
    cycle-consistent adversarial networks for image super-resolution,
    cycle-consistent adversarial networks for image inpainting,
  ]
---

> Citations: 8,605 | Paper Published: 01 Oct 2017 | Institutions: University of California, Berkeley| Authors: Jun-Yan Zhu, Taesung Park, Phillip Isola, Alexei A. Efros

<!-- Prettier doesn't change this -->

:::tip Abstract in 2 Lines

The paper presents an approach for image-to-image translation without paired training data. The approach uses an adversarial loss and a cycle consistency loss to learn a mapping between two domains.

:::

## Contributions

- An approach for image-to-image translation without paired training data.
- The use of an adversarial loss and a cycle consistency loss to learn a mapping between two domains.
- Qualitative results on several tasks where paired training data does not exist, including collection style transfer, object transfiguration, season transfer, photo enhancement, etc.
- Quantitative comparisons against several prior methods demonstrate the superiority of the proposed approach.


## Practical Implications

- The proposed approach can be used for image-to-image translation tasks where paired training data is not available.
- The approach can be used for various tasks such as collection style transfer, object transfiguration, season transfer, photo enhancement, etc.
- The approach can be used to generate high-quality images that are indistinguishable from the target domain.
- The proposed approach outperforms several prior methods in terms of quantitative metrics.


## Methods

<!-- Prettier doesn't change this -->

:::info Methodology


- Adversarial loss: The approach uses an adversarial loss to learn a mapping between two domains. The goal is to learn a mapping G : X → Y such that the distribution of images from G(X) is indistinguishable from the distribution Y.
- Cycle consistency loss: Because the mapping is highly under-constrained, the approach couples it with an inverse mapping F : Y → X and introduces a cycle consistency loss to push F(G(X)) ≈ X (and vice versa).
- Unpaired image-to-image translation: The approach learns to translate an image from a source domain X to a target domain Y in the absence of paired examples.

:::

## Data

- Cityscapes: A dataset of urban street scenes.
- Maps: A dataset of maps and aerial photographs.
- Yosemite: A dataset of Yosemite National Park.
- Edges2Shoes: A dataset of shoe images and their edge maps.
- Edges2Handbags: A dataset of handbag images and their edge maps.


## Results

<!-- Prettier doesn't change this -->

:::note Performance Analysis

- Cityscapes dataset: The proposed approach achieves a PSNR of 27.3, an SSIM of 0.86, and an FID of 27.5.
- Maps dataset: The proposed approach achieves a PSNR of 26.5, an SSIM of 0.85, and an FID of 29.6.
- Yosemite dataset: The proposed approach achieves a PSNR of 28.1, an SSIM of 0.92, and an FID of 16.8.
- Edges2Shoes dataset: The proposed approach achieves a PSNR of 28.3, an SSIM of 0.91, and an FID of 22.4.
- Edges2Handbags dataset: The proposed approach achieves a PSNR of 27.9, an SSIM of 0.90, and an FID of 27.5.

:::

## Limitations

One limitation of this paper is that the proposed approach requires a large amount of training data to learn the mapping between the source and target domains. Another limitation is that the approach may not work well for complex image-to-image translation tasks where the source and target domains are very different from each other. Additionally, the approach may not be suitable for real-time applications due to its high computational cost. Finally, the approach may generate images that are not semantically meaningful or visually realistic in some cases.
