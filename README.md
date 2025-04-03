# Malaria Cell Image Classification with Hybrid CNN Model (Spatial Pyramid Pooling Approach)

## Overview
This project presents a **hybrid CNN-Transformer model** for **Malaria cell image classification**, integrating **custom CNN architecture with EfficientNetB0** and enhanced by **CBAM Attention Mechanism, Residual Learning, and ASPP (Atrous Spatial Pyramid Pooling)**. The model achieves **high classification accuracy**, ensuring robust detection of malaria from cell images.

## Model Architecture
- **Custom CNN Branch**: Extracts low- and mid-level image features.
- **CBAM Attention Mechanism**: Enhances feature representation by focusing on important spatial and channel-wise information.
- **Residual Blocks**: Helps mitigate vanishing gradients and improves feature learning.
- **ASPP (Atrous Spatial Pyramid Pooling)**: Captures multi-scale contextual information.
- **EfficientNetB0 Backbone**: Pretrained model for high-level feature extraction.
- **Feature Fusion**: Merges features from **CNN and EfficientNetB0** before classification.

## Performance Metrics
| Class        | Precision | Recall | F1-Score | Support |
|-------------|-----------|--------|----------|---------|
| Parasitized | 0.97      | 0.96   | 0.97     | 1402    |
| Uninfected  | 0.96      | 0.97   | 0.97     | 1356    |
| **Accuracy**  | **0.97** | -      | -        | **2758**  |
| **Macro Avg** | 0.97      | 0.97   | 0.97     | 2758    |
| **Weighted Avg** | 0.97  | 0.97   | 0.97     | 2758    |

## Results
- **Training Accuracy**: 99.15%
- **Validation Accuracy**: 96.37%
- **Testing Accuracy**: 96.59%
