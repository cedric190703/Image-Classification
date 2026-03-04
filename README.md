# Ship Image Classification -- CNN (Top 3 / 117 Teams)

## Overview

This project was developed as part of an internal Kaggle competition.
The objective was to classify ship images into multiple categories using
a Convolutional Neural Network (CNN).

**Constraint:** The model had to contain fewer than **30 layers**.

🏆 **Final Ranking:** Top 3 out of 117 teams
📊 **Validation Score:** 0.87174

------------------------------------------------------------------------

## Team

-   Cédric Brzyski
-   Tom Coulliaud-Maisonneuve

------------------------------------------------------------------------

## Approach

We designed a custom CNN architecture using **TensorFlow, Keras**,
optimized for high performance under architectural constraints.

### Key Components:

-   Custom CNN (< 30 layers)
-   Batch Normalization
-   L2 Regularization
-   Data Augmentation:
    -   Random horizontal flips
    -   Brightness and contrast adjustments
    -   Saturation and hue variations
-   Multi-stage training strategy
-   Learning rate scheduling
-   EarlyStopping
-   ModelCheckpoint

------------------------------------------------------------------------

## Model Architecture

-   Input: 64x64 RGB images
-   Convolutional blocks with BatchNorm
-   Progressive feature extraction
-   Fully connected classifier
-   Loss: Sparse Categorical Cross-Entropy
-   Optimizer: Adam

The architecture was carefully tuned to balance:

-   Model capacity
-   Overfitting control
-   Training stability
-   Competition constraints

------------------------------------------------------------------------

## Training Strategy

To maximize generalization performance:

-   Progressive learning rate decay
-   Regularization techniques
-   Hyperparameter tuning
-   Validation monitoring to prevent overfitting

------------------------------------------------------------------------

## Tech Stack

-   Python
-   TensorFlow
-   Keras
-   NumPy
-   Matplotlib
