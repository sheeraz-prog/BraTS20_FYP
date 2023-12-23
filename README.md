# Brain Tumor Segmentation and Overall Survival Prediction

## Overview

This project focuses on the segmentation of brain tumors using a 3D Unet model and predicts overall survival using an Ensemble Machine Learning approach. The dataset used for training and evaluation is the BraTS20 dataset, which provides MRI scans along with ground truth masks.

## Segmentation (3D Unet Model)

### Model Architecture

The segmentation task is accomplished using a 3D Unet model. The architecture is designed to capture intricate spatial features and accurately segment tumor regions in 3D MRI scans.

### Training

The model is trained on the BraTS20 dataset, which includes pre-processed MRI scans and corresponding segmented masks. The training process involves optimizing the model to learn features representative of tumor structures.

## Overall Survival Prediction (Ensemble Machine Learning)

### Ensemble Approach

For predicting overall survival, an Ensemble Machine Learning approach is adopted. The ensemble is composed of multiple machine learning models, each contributing to the final prediction. Common models like Random Forest, SVM, and Decision Trees are utilized.

### Feature Extraction

Radiomic features are extracted from segmented tumor regions. These features capture characteristics such as tumor size, shape, area, perimeter, texture, location, and intensity. The ensemble is trained on these features to predict overall survival.

## Usage

### Segmentation

1. **Training:** Execute the training script for the 3D Unet model on the BraTS20 dataset.
2. **Inference:** Use the trained model for segmenting brain tumors in new MRI scans.

### Survival Prediction

1. **Feature Extraction:** Extract radiomic features from segmented tumor regions.
2. **Training:** Train the Ensemble Machine Learning model on the extracted features.
3. **Prediction:** Utilize the trained ensemble for predicting overall survival.

## Dependencies

- Python 3.x
- TensorFlow
- scikit-learn
- SimpleITK
- Radiomics

## Contributions

Contributions and feedback are welcome! If you have suggestions or would like to contribute, please open an issue or create a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
