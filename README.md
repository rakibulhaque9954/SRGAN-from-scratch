# SRGAN-from-scratch

## Introduction
This Jupyter notebook is a comprehensive guide to building a Super-Resolution Generative Adversarial Network (SRGAN) from the ground up. The focus is on upscaling 64x64 pixel images to 256x256 pixels, using the "mirflickr" dataset for training. This project highlights the practical application of deep learning for image super-resolution tasks.

## Model Overview

### SRGAN Architecture
The SRGAN model consists of two main components:
- **Generator**: Enhances the resolution of images.
- **Discriminator**: Judges the authenticity of the super-resolved images against the original high-resolution images.

### Dataset
Training leverages the "mirflickr" dataset, a diverse collection of images perfect for super-resolution challenges.

## Training Process

### Initial Training
Started with 12,500 images across 9 epochs, the initial training achieved a PSNR value of 28.5, indicating the model's potential for high-quality image generation.

### Extended Training
Progressing with 25,000 images over a span of 3 days, the model's PSNR improved to 29.35, showcasing enhanced performance and learning.

## Implementation Details

### Generator and Discriminator Networks
The notebook contains the architecture and code for both the generator and discriminator, explaining the design, loss functions, training loops, and metrics.

### Single GPU Training
The model was trained on an A100 GPU for 3 days, balancing computational efficiency with resource availability.

## Results

### Performance
The results indicate that the SRGAN model is capable of significantly improving the resolution of images. Despite the limitations in training duration and dataset size, the PSNR values are promising.

### Quality of Super-Resolved Images
The super-resolved images show a considerable enhancement in quality from their low-resolution counterparts. The transition from 64x64 to 256x256 pixels demonstrates the model's effectiveness.

### Visual Results
Below is a screenshot from the notebook that provides a visual comparison between the low-resolution (LR), the super-resolved (SR) by our model, and the original high-resolution (HR) images. This illustrates the effectiveness of the SRGAN model in enhancing image detail and quality.

![Comparison of LR, SR, and HR Images](https://github.com/rakibulhaque9954/SRGAN-from-scratch/blob/2b2b85de697738a6e4c2e7ae381eba528ad83dc9/Screenshot%202023-10-05%20at%2008.04.18.png)
*From left to right: Low-Resolution (LR) image, Super-Resolved (SR) image by SRGAN, and the Original High-Resolution (HR) image.*

### Generator Summary Screenshot
The notebook includes a detailed summary of the generator's architecture, as shown in the screenshot below:
![Generator Summary Screenshot](path_to_generator_summary_screenshot.png)

## How to Use This Notebook

### Prerequisites
Ensure you have the necessary hardware and software setup, including access to a GPU for training (ideally an A100).

### Downloading the Dataset
The "mirflickr" dataset can be downloaded from Kaggle. Follow these steps to get started:
1. Visit the Kaggle website and search for the "mirflickr" dataset.
2. Download the dataset to your local machine.
3. Unzip the dataset into a directory that your Jupyter notebook can access.

### Running the Notebook
Follow the instructions and code within the notebook step-by-step to replicate the model training or to perform super-resolution on your images.

## Conclusion
The SRGAN model shows promising results in super-resolution imaging. Further improvements could be made by extending training time, enlarging the dataset, and refining the model's architecture.

