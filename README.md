# Live Fence Detection using Vision Transformers

This repository contains a complete deep learning pipeline for detecting Live Fences (linear arrangements of trees and shrubs in agricultural landscapes) from satellite imagery using Vision Transformers (ViT).

## Overview

Live Fences are important landscape features that provide ecological connectivity, reduce erosion, and support biodiversity conservation in agricultural areas. This project implements a complete pipeline from preprocessing satellite imagery to classification and evaluation.

## Pipeline Components

1. **Preprocessing Pipeline**: Validates and normalizes multi-band satellite imagery
2. **Vision Transformer Classification**: Trains a ViT model to classify Live Fences
3. **Results Analysis**: Evaluates model performance with detailed metrics and visualizations

## Notebooks

The workflow is implemented as a series of Google Colab notebooks:

- [01_preprocessing_pipeline.ipynb](https://colab.research.google.com/drive/1ke1LxLKKPliwH_t4ltZRElQoK_dbBndJ#scrollTo=4IUTFZBA0Bd_) - Data validation and normalization
- [02_vit_classification.ipynb](https://colab.research.google.com/drive/1cUGDakSMNjGWSJVtbAED1kmQDpydGyQ4#scrollTo=2AjuPTELgyYq) - ViT model implementation and training
- [03_results_analysis.ipynb](https://colab.research.google.com/drive/1yBlZyovEwEYL1CF42_axUUhWQFDvVXpy#scrollTo=Ze_CRhu2huFD) - Detailed performance evaluation

## Dataset

The model is trained on 4-band (RGB+NIR) satellite imagery of agricultural landscapes. Each image is labeled as either containing a Live Fence (AF) or not (noAF).


For detailed analysis, see the [results documentation](docs/results.md).

## Installation

```bash
pip install -r requirements.txt