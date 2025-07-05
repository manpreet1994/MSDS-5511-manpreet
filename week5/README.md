# Generative Adversarial Networks for Image Style Transfer (Monet-Style Image Generation)

This repository focuses on image generation using Generative Adversarial Networks (GANs), with a specific objective of transforming images into the distinctive style of Claude Monet. The project explores and compares two prominent GAN architectures: Deep Convolutional Generative Adversarial Networks (DCGANs) and Cycle-Consistent Generative Adversarial Networks (CycleGANs). Although the implement only contains CycleGANs.

## Project Objective

The primary goal of this project was to generate images in the artistic style of Claude Monet from a given set of input images. This involves learning the characteristic features and brushstrokes of Monet's paintings and applying them to new visual data.

## Methodologies Explored

### 1. Deep Convolutional Generative Adversarial Network (DCGAN)

* **Approach:** An initial attempt involved training a DCGAN to produce Monet-style images.
* **Challenges:** Despite extensive training over multiple days and numerous epochs, the DCGAN architecture encountered significant issues with mode collapse.
* **Outcome:** Mode collapse led to a severe lack of diversity in the generated outputs, with the model consistently producing a limited set of repetitive and undifferentiated images. Consequently, the DCGAN did not meet the project's objectives effectively.

### 2. Cycle-Consistent Generative Adversarial Network (CycleGAN)

* **Approach:** Following the difficulties with DCGAN, the project transitioned to implementing a CycleGAN.
* **Effectiveness:** The CycleGAN architecture proved to be highly effective in addressing the challenges faced by DCGAN.
* **Outcome:** This model successfully generated diverse and visually compelling images that accurately captured the distinctive style of Claude Monet. The CycleGAN demonstrated a robust ability to translate source images into the target style, producing high-quality outputs without suffering from mode collapse.

## Key Findings

The transition from DCGAN to CycleGAN was crucial for the success of this project. While DCGAN struggled with generating diverse outputs due to mode collapse, CycleGAN effectively overcame this limitation, proving to be a powerful architecture for image-to-image translation tasks, particularly for artistic style transfer.