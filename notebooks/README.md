# Notebooks

This directory contains the primary Jupyter notebooks used for the development, training, evaluation, and explainability analysis of the proposed XAI-HybridNet framework.

## Files

### `XAI_HybridNet.ipynb`
Main implementation notebook containing:
- Dataset preprocessing and augmentation
- ResNet-50 and ViT-B/16 model training
- Hybrid ensemble fusion
- Explainability generation using Grad-CAM, Guided Grad-CAM, SHAP, LIME, and attention maps
- Hybrid multimodal explanation generation
- Quantitative evaluation and statistical analysis

### `Hybridnet_metrics.ipynb`
Supplementary notebook for:
- Performance metric computation
- Consensus and stability analysis
- XCS and X-Entropy evaluation
- McNemar statistical significance testing
- Visualization and graph generation

## Notes

- The notebooks were developed using PyTorch with CUDA acceleration.
- Dataset paths may need to be updated based on local directory structure.
- Pretrained ImageNet weights are used for ResNet-50 and ViT-B/16 initialization.
- Generated outputs and visualizations are stored within the `results/` directory.

## Recommended Environment

- Python 3.10+
- PyTorch
- torchvision
- timm
- OpenCV
- SHAP
- LIME
- matplotlib
- scikit-learn
