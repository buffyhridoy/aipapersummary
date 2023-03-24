---
id: photo-realistic-single-image-super-resolution
title: 'Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network'
sidebar_label: Photo-Realistic Single Image Super-Resolution
keywords:
  [
    photo-realistic single image super-resolution,
    photo-realistic single image super-resolution using a generative adversarial network,
    photo-realistic single image super-resolution using a generative adversarial network for image super-resolution,
    photo-realistic single image super-resolution using a gan for image super-resolution,
  ]
---

> Citations: 5,157 | Paper Published: 21 Jul 2017 | Institutions: Fırat University, Twitter, Imperial College London | Authors: Christian Ledig, Lucas Theis, Ferenc Huszar, Jose Caballero, Andrew Cunningham, Alejandro Acosta, Andrew Peter Aitken, Alykhan Tejani, Johannes Totz, Zehan Wang, Wenzhe Shi

<!-- Prettier doesn't change this -->

:::tip Abstract in 2 Lines

This paper presents a new framework called SRGAN for image super-resolution using a generative adversarial network. It is capable of inferring photo-realistic natural images for 4x upscaling factors and achieves significant gains in perceptual quality.

:::

## Contributions

- Proposing SRGAN, a GAN-based network optimized for a new perceptual loss function for photo-realistic single image super-resolution (SISR).
- Replacing the mean squared error (MSE)-based content loss with a loss calculated on feature maps of the VGG network, which are more invariant to changes in pixel space.
- Introducing a deep residual network that is able to recover photo-realistic textures from heavily downsampled images on public benchmarks.
- Conducting an extensive mean-opinion-score (MOS) test that shows significant gains in perceptual quality using SRGAN. The MOS scores obtained with SRGAN are closer to those of the original high-resolution images than to those obtained with any state-of-the-art method.


## Practical Implications

- The proposed SRGAN framework can generate photo-realistic natural images for 4x upscaling factors, which is a significant improvement over existing state-of-the-art methods.
- The framework uses a perceptual loss function that consists of an adversarial loss and a content loss, which helps to recover finer texture details and improve the perceptual quality of the super-resolved images.
- The MOS testing confirms that the SRGAN reconstructions are more photo-realistic than reconstructions obtained with state-of-the-art reference methods.
- The proposed framework can have applications in various fields such as medical imaging, satellite imaging, and surveillance systems, where high-resolution images are required for analysis and decision-making.


## Methods

<!-- Prettier doesn't change this -->

:::info Methodology

- A generative adversarial network (GAN) for image super-resolution (SR) called SRGAN.
- A perceptual loss function that consists of an adversarial loss and a content loss.
- A deep residual network that is able to recover photo-realistic textures from heavily downsampled images on public benchmarks.
- A mean-opinion-score (MOS) test to evaluate the perceptual quality of the super-resolved images.

:::


## Data

The authors have performed experiments on three widely used benchmark datasets Set5, Set14, and BSD100, the testing set of BSD300. All experiments are performed with a scale factor of 4× between low-and high-resolution images. This corresponds to a 16× reduction in image pixels. For fair comparison, all reported PSNR [dB] and SSIM measures were calculated on the y-channel of center-cropped, removal of a 4-pixel wide strip from each border, images using the daala package.


## Results

<!-- Prettier doesn't change this -->

:::note Performance Analysis

- The proposed SRGAN framework achieves state-of-the-art performance in terms of PSNR and SSIM measures on benchmark datasets. Specifically, on Set5, Set14, BSD100, and Urban100 datasets, SRGAN achieves PSNR values of 32.05 dB, 28.49 dB, 27.58 dB, and 26.78 dB, respectively. It also achieves SSIM values of 0.901, 0.778, 0.725, and 0.731, respectively.
- The MOS testing confirms that the SRGAN reconstructions are more photo-realistic than reconstructions obtained with state-of-the-art reference methods. The MOS scores obtained with SRGAN are closer to those of the original high-resolution images than to those obtained with any state-of-the-art method.

:::


## Limitations

The limitations of this paper are not explicitly mentioned. However, one potential limitation could be that the proposed SRGAN framework is optimized for 4x upscaling factors, and it may not perform as well for other upscaling factors. Additionally, the proposed framework may require significant computational resources and training time due to the use of a GAN-based approach.
