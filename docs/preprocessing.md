# Preprocessing Pipeline

## Overview

The preprocessing pipeline handles satellite imagery validation, normalization, and preparation for deep learning models. It is specifically designed for 4-band (RGB+NIR) imagery used for Live Fence detection.

## Key Components

### Image Validation

Images are validated using multiple criteria:
- Correct dimensions (128x128 pixels)
- Presence of all four spectral bands
- Absence of NaN/Inf values
- Absence of empty bands

### Band Normalization

Each spectral band is normalized using:
- Percentile-based clipping (2-98%)
- Statistical outlier removal
- Linear scaling to [0,1] range
- Band-specific adjustments for feature enhancement

### Dataset Preparation

The preprocessing workflow includes:
- Calculation of global band statistics
- Consistent normalization across the dataset
- Stratified split into training, validation, and test sets

## Class Structure

The `DatasetPreprocessor` class implements the complete pipeline with detailed error tracking and validation at each step.

## Usage Examples

```python
# Initialize preprocessor
preprocessor = DatasetPreprocessor(folder_paths, class_names)

# Load and preprocess dataset
X_train, X_val, X_test, y_train, y_val, y_test, images, labels = prepare_dataset_for_deep_learning(
    folder_paths, class_names
)