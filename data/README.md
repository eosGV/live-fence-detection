# Dataset Information

This file explains the structure of the dataset used for Live Fence detection.

## Data Source

The dataset consists of 4-band (RGB+NIR) satellite imagery from Planet's PlanetScope constellation with 3-meter resolution, acquired over agricultural landscapes.

## Dataset Structure

The dataset is organized as follows:
- `AF/`: Contains images with Live Fences
- `noAF/`: Contains images without Live Fences

Each image is a 128x128 pixel tile representing approximately 384x384 meters on the ground.

## Preprocessing

The preprocessing steps applied to these images include:
1. Validation (dimensions, band availability, outlier check)
2. Normalization of each spectral band
3. Statistical outlier removal
4. Split into training, validation, and test sets

## Statistics

- Total images: 777
- AF class: 597 images
- noAF class: 180 images
- Training set: 543 images
- Validation set: 117images
- Test set: 117 images