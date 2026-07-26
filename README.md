# Cat Skin Disease Classification

This project aims to classify common skin diseases in cats using deep learning. A TensorFlow/Keras model was trained to identify four different skin conditions from cat skin images.

## Classes

The model predicts one of the following classes:

- Health
- Flea Allergy
- Ringworm
- Scabies

## Dataset

The dataset is organized into four class folders. During preprocessing, the dataset is automatically split into training, validation and test sets.

Before training, the following preprocessing steps are applied:

- Resize images to **224 × 224**
- Normalize pixel values
- Data augmentation
  - Random Flip
  - Random Rotation
  - Random Zoom
  - Random Contrast

## Model

The model is implemented using **TensorFlow/Keras**. After training, the best performing model is saved as:

```text
best_cat_skin_model.keras
```

The saved model can be loaded later to classify new images without retraining.

## Libraries

The project mainly uses:

- TensorFlow
- NumPy
- Matplotlib
- pathlib

## Workflow

1. Load and extract the dataset.
2. Split the dataset into training, validation and test sets.
3. Create TensorFlow datasets.
4. Apply data augmentation.
5. Train the model.
6. Save the best model.
7. Load the saved model for prediction.

---
This project was developed for educational purposes as part of a deep learning and computer vision study.
