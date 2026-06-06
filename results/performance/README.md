# Performance Evaluation Results

This folder contains quantitative evaluation, statistical benchmarking, calibration analysis, and optimization behavior of the proposed XAI-HybridNet framework.

## Included Figures

### metric_comparison.png
Comparative performance analysis of ResNet-50, ViT-B/16, and HybridNet across Accuracy, Precision, Recall, and F1-score metrics. The proposed HybridNet demonstrates improved overall balance between sensitivity and classification robustness.

### mcnemar_analysis.png
McNemar statistical comparison illustrating disagreement analysis between HybridNet and the baseline architectures. The figure highlights the number of corrected baseline errors and remaining HybridNet errors for each model comparison.

### resnet_training_accuracy.png
Training and validation accuracy curves for ResNet-50 across optimization epochs. The figure illustrates convergence behavior and validation performance trends during training.

### resnet_training_loss.png
Training and validation loss curves for ResNet-50 showing optimization dynamics and gradual divergence between training and validation loss at later epochs.

### reliability_calibration.png
Reliability calibration diagram comparing confidence calibration across ResNet-50, ViT-B/16, and HybridNet. Expected Calibration Error (ECE) values indicate that HybridNet achieves the best confidence calibration among the evaluated models.

### faithfulness_evaluation.png
Faithfulness deletion and insertion evaluation curves used to assess explanation reliability. The deletion test evaluates how rapidly prediction confidence decreases when important regions are removed, while the insertion test evaluates confidence recovery when informative regions are progressively restored.
