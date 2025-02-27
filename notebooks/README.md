### notebooks/README.md
```markdown
# Notebooks

This directory contains links to Google Colab notebooks that implement the Live Fence detection pipeline.

## Preprocessing Pipeline

[01_preprocessing_pipeline.ipynb](https://colab.research.google.com/drive/1ke1LxLKKPliwH_t4ltZRElQoK_dbBndJ#scrollTo=4IUTFZBA0Bd_)

This notebook implements the data preprocessing pipeline including:
- Image validation with custom error tracking
- Adaptive band normalization for RGB+NIR data
- Complete preprocessing pipeline from raw data to ML-ready datasets

## Vision Transformer Classification

[02_vit_classification.ipynb](https://colab.research.google.com/drive/1cUGDakSMNjGWSJVtbAED1kmQDpydGyQ4#scrollTo=2AjuPTELgyYq)

This notebook implements the Vision Transformer model including:
- Custom ViT implementation for satellite imagery
- Transfer learning strategies
- Training process with callbacks and visualizations

## Results Analysis

[03_results_analysis.ipynb](https://colab.research.google.com/drive/1yBlZyovEwEYL1CF42_axUUhWQFDvVXpy#scrollTo=Ze_CRhu2huFD)

This notebook provides detailed analysis of model performance:
- Confusion matrix and classification metrics
- ROC and Precision-Recall curves
- Visualization of model predictions
- Discussion of ecological implications