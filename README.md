# XAI-HybridNet

## Trustworthy Hybrid CNN–Transformer Framework for Explainable Medical Image Analysis

XAI-HybridNet is a unified explainability-oriented deep learning framework designed for interpretable pneumonia detection from pediatric chest X-ray images. The framework combines the localized spatial learning capability of CNNs with the global contextual reasoning strengths of Vision Transformers through weighted ensemble fusion and multimodal explainability integration.

The proposed framework integrates:
- ResNet-50 and ViT-B/16 hybrid ensemble learning
- Grad-CAM and Guided Grad-CAM localization
- Vision Transformer attention visualization
- SHAP and LIME model-agnostic explanations
- Hybrid multimodal explanation fusion
- Cross-method explainability reliability evaluation using XCS and X-Entropy metrics

---

# Architecture Overview

<p align="center">
  <img src="results/explainability/architecture.png" width="850">
</p>

The framework combines:
1. Image preprocessing and augmentation
2. Parallel feature extraction using ResNet-50 and ViT-B/16
3. Weighted probability fusion
4. Hybrid explainability generation
5. Cross-method reliability and consensus evaluation

---

# Experimental Datasets

The framework was evaluated using two publicly available pediatric chest X-ray datasets.

| Dataset | Normal | Pneumonia | Total | Contribution |
|---|---|---|---|---|
| Kaggle Chest X-ray | 1,583 | 4,273 | 5,856 | 69.4% |
| Mendeley Chest X-ray | 1,320 | 1,306 | 2,626 | 31.1% |
| **Combined Dataset** | **2,895** | **5,541** | **8,436** | **100%** |

## Dataset Sources

### Kaggle Pediatric Chest X-ray Dataset
https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

### Mendeley Chest X-ray Dataset
https://data.mendeley.com/datasets/wndbd5r26y/3

---

# Performance Evaluation

## Quantitative Performance Comparison

<p align="center">
  <img src="results/performance/metric_comparison.png" width="750">
</p>

| Model | Accuracy | Precision | Recall | F1-score |
|---|---|---|---|---|
| ResNet-50 | 0.816 | 0.813 | 0.879 | 0.845 |
| ViT-B/16 | 0.832 | 0.851 | 0.854 | 0.853 |
| **HybridNet (Proposed)** | **0.845** | **0.855** | **0.875** | **0.859** |

The proposed XAI-HybridNet framework achieved improved predictive stability and balanced classification performance while maintaining strong recall characteristics important for pneumonia detection tasks.

---

# Statistical Significance Analysis

## McNemar Test Comparison

<p align="center">
  <img src="results/performance/mcnemar_analysis.png" width="750">
</p>

The McNemar statistical analysis demonstrates comparative disagreement distributions between HybridNet and the baseline architectures, supporting the evaluation of predictive robustness and ensemble consistency.

---

# Explainability Outputs

## Grad-CAM Visualization

<p align="center">
  <img src="results/explainability/gradcam_visualization.png" width="280">
</p>

Grad-CAM highlights localized pulmonary regions contributing strongly to the classification decision.

---

## Vision Transformer Attention Map

<p align="center">
  <img src="results/explainability/vit_attention_map.png" width="280">
</p>

ViT attention visualization captures broader global contextual dependencies across chest radiographs.

---

## Hybrid Attention Fusion

<p align="center">
  <img src="results/explainability/hybrid_attention_map.png" width="280">
</p>

The hybrid attention map combines CNN localization with transformer contextual reasoning to produce smoother and more coherent explanations.

---

## SHAP Attribution Analysis

<p align="center">
  <img src="results/explainability/shap_attribution_analysis.png" width="280">
</p>

SHAP provides pixel-level attribution analysis for model-agnostic interpretability assessment.

---

## LIME Superpixel Explanation

<p align="center">
  <img src="results/explainability/lime_superpixel_explanation.png" width="280">
</p>

LIME generates local superpixel explanations that highlight clinically relevant image regions influencing predictions.

---

# Failure Case Analysis

<p align="center">
  <img src="results/failure_cases/false_positive_case1.png" width="350">
</p>

Representative failure cases indicate that subtle pulmonary intensity variations and overlapping anatomical structures may occasionally resemble pneumonia-related opacity patterns, resulting in false-positive predictions.

---

# Installation

Clone the repository:

```bash
git clone https://github.com/nomadcodin/XAI_HybridNet.git
cd XAI_HybridNet
