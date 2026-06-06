# Architecture

This directory contains the system architecture diagram of the proposed XAI-HybridNet framework for explainable pneumonia detection from chest X-ray images.

## Files

### `architecture.png`

The architecture diagram illustrates the complete workflow of the proposed explainability-oriented hybrid framework, including:

- Chest X-ray dataset input
- Image preprocessing and augmentation
- Parallel feature extraction using ResNet-50 and ViT-B/16
- Hybrid ensemble prediction generation
- Unified multimodal explainability pipeline
- LIME superpixel explanation generation
- SHAP pixel attribution analysis
- Hybrid visual explanation fusion

The framework combines CNN-based local spatial feature extraction with transformer-based global contextual reasoning to improve both predictive performance and interpretability in medical image analysis.

## Workflow Summary

The pipeline consists of four major stages:

1. **Data Preparation**
   - Chest X-ray image acquisition
   - Resizing, normalization, and augmentation

2. **Hybrid Feature Learning**
   - Parallel feature extraction using ResNet-50 and ViT-B/16
   - Ensemble fusion for final prediction generation

3. **Explainability Integration**
   - Grad-CAM localization
   - LIME superpixel explanations
   - SHAP attribution analysis
   - Transformer attention visualization

4. **Unified Interpretation**
   - Hybrid multimodal explanation generation
   - Interpretable prediction support for clinical analysis

## Purpose

The architecture diagram provides a high-level overview of how deep learning classification and multiple explainability mechanisms are integrated within a unified medical image analysis framework. The figure serves as the primary visual summary of the proposed XAI-HybridNet system throughout the repository and accompanying research manuscript.
