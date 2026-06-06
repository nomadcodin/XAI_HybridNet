# Explainability Consensus and Stability Analysis

This folder contains quantitative explainability reliability evaluation results using the proposed X-Consensus Score (XCS) and X-Entropy stability metrics.

## Included Figures

### xcs_xentropy_overview.png
Overview comparison of X-Consensus Score (XCS) and X-Entropy metrics across ResNet-50, ViT-B/16, and HybridNet. Higher XCS indicates stronger cross-method explanation agreement, while lower X-Entropy indicates improved explanation stability.

### per_sample_xcs_analysis.png
Per-sample explainability consensus analysis across randomly selected test samples. HybridNet consistently demonstrates higher cross-method explanation agreement compared to the baseline architectures.

### per_sample_xentropy_analysis.png
Per-sample X-Entropy evaluation illustrating explanation uncertainty and stability across multiple test samples. Lower X-Entropy values observed for HybridNet indicate more stable and coherent explanations.
