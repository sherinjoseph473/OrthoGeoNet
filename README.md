# OrthoGeoNet

**Automated Calcaneal Pitch Angle Estimation and Flatfoot Severity Assessment Using Deep Learning**

## About

OrthoGeoNet is a deep learning framework for estimating the calcaneal pitch angle and assessing flatfoot severity from weight-bearing lateral foot X-ray images. It identifies four anatomical landmarks, calculates the angle geometrically, and categorizes the foot as severe flatfoot, moderate flatfoot, or normal.

## Dataset

- **Total images:** 540 foot radiographs
- **Total subjects:** 272
- **Training set:** 378 images
- **Validation set:** 82 images
- **Testing set:** 80 images

The dataset was divided at the subject level to prevent images from the same subject from appearing in different subsets.

## Methodology

OrthoGeoNet integrates the following components:

- Anatomical Structure Enhancement Module (ASEM)
- ConvNeXt V2 with Feature Pyramid Network (FPN)
- Vision Mamba for global feature representation
- Heatmap-based anatomical landmark localization
- Geometric calcaneal pitch angle estimation

## Results

The paper reports the following results on the independent test set:

| Evaluation Metric | Result |
|---|---:|
| Landmark localization MAE | 1.27 pixels |
| Landmark localization RMSE | 1.61 pixels |
| Calcaneal pitch angle MAE | 0.71° |
| Calcaneal pitch angle RMSE | 0.94° |
| Severity classification accuracy | 95.00% |

*Note: These are the results reported in the paper and have not necessarily been independently reproduced by the repository implementation.*

## Technologies

- Python
- PyTorch
- NumPy
- Pandas
- OpenCV
- Scikit-learn

## Repository Status

This repository is intended to provide the implementation, training and evaluation procedures, and inference utilities for the proposed OrthoGeoNet framework.

## Disclaimer

This project is intended for research and educational purposes only. It is not a substitute for professional medical assessment or diagnosis.

