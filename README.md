# CycleGAN for Image-to-Image Translation 

This repository contains an implementation of a **Cycle-Consistent Generative Adversarial Network (CycleGAN)**, modeled for the Kaggle competition *I'm Something of a Painter Myself*. 

CycleGAN is specifically designed for unpaired image-to-image translation tasks. It enables seamless domain mapping without the need for paired datasets, making it ideal for applications such as style transfer, domain adaptation, and artistic image generation.

## Overview

CycleGAN addresses the challenge of translating images between two domains A and B, ensuring that:

- **Realism**: The translated images appear natural and convincing.
- **Content Preservation**: Key details from the source domain are maintained in the translated image.

CycleGAN achieves this by introducing **cycle consistency loss**, which enforces that translating an image from (A to B to A) or  (B to A to B)  yields an image close to the original input.

## Key Features

- **Unpaired Training**: Train on unpaired datasets, making it applicable to diverse domains.
- **Cycle Consistency Loss**: Ensures that the generated mappings are meaningful and not arbitrary.
- **Discriminator Loss**: Evaluates the realism of generated images.


## Notebook Overview

This repository includes the following files:

- `CycleGAN.ipynb`: A complete implementation of CycleGAN with the following features:
  - Dataset loading and preprocessing.
  - Implementation of the Generator and Discriminator networks.
  - Cycle-consistency loss computation.
  - Training loop with metrics and visualizations.

### Dependencies

To run the notebook, ensure the following libraries are installed:

- TensorFlow / PyTorch
- NumPy
- Matplotlib
- PIL (Pillow)
- Jupyter Notebook

Install them via:
```bash
pip install tensorflow numpy matplotlib pillow
