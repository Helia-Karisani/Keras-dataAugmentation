# Data Augmentation with Keras

This project applies **data augmentation** in Keras to expand an image dataset. By transforming existing images, the model sees more variations, which helps it generalize better during training.

---

## Overview

The notebook prepares image data for training by generating modified versions of the same image. Instead of collecting more data, augmentation creates new samples from existing ones.

This is especially useful with **small datasets**, where models tend to overfit.

---

## Core Idea

Data augmentation applies random transformations to images while keeping their meaning.

Transformations used:

- rotation
- shifting
- zooming
- flipping
- rescaling

---

## Workflow

1. Load an image
2. Convert it into a format suitable for processing
3. Apply augmentation transformations
4. Generate multiple variations of the same image
5. Visualize the augmented outputs

---

## Example Image

The input image used for augmentation:

![Sample image](sample.jpg)

---

## Augmentation Process

An image generator is defined in Keras with transformation parameters. Each time the generator is used, it produces a slightly different version of the same image, so the dataset grows without adding new raw data.

Main benefits: less overfitting, better generalization, and more robustness to real-world variation.

---

## File Structure

```
Keras-dataAugmentation.ipynb   # main notebook
sample.jpg                     # input image used for augmentation
README.md
```
