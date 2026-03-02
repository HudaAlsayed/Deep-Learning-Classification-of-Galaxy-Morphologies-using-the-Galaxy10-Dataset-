# Deep-Learning-Classification-of-Galaxy-Morphologies-using-the-Galaxy10-Dataset-
Deep learning project for classifying galaxy morphologies using the Galaxy10 dataset (21,785 images). Built a CNN with data augmentation and stratified splitting to address class imbalance. Achieved 84% test accuracy and evaluated performance using a confusion matrix for detailed class-level analysis.
This project implements a deep learning pipeline to classify galaxy images into 10 morphological types using the Galaxy10 dataset. The goal is to automate galaxy classification using Convolutional Neural Networks (CNNs) while addressing real-world challenges such as class imbalance.

- Dataset

Dataset: Galaxy10

Total Images: 21,785

Image Size: 69 × 69 × 3 (RGB)

Classes: 10 galaxy morphological types (labels 0–9)

The dataset exhibits severe class imbalance, which was carefully handled during training and evaluation.

- Project Pipeline
1️) Data Preprocessing

Stratified 80/20 train-test split

Z-score standardization (training statistics only)

One-hot encoding of labels

Data augmentation (rotation, zoom, shifts)

2) Model Architecture

Custom CNN (Galaxy10CNN)

3 Convolutional layers + ReLU

MaxPooling layers

Fully connected layer

Softmax output (10 classes)

Optimizer: Adam

Loss Function: Categorical Cross-Entropy

Training: 50 epochs

3) Evaluation

Test Accuracy: 84%

Confusion Matrix for detailed class-level performance analysis

Focus on identifying misclassifications in minority classes

- System Workflow

Galaxy Image → Standardization → Data Augmentation → CNN Model → 10-Class Output → Evaluation Metrics

- Results

Successfully built an end-to-end deep learning pipeline

Improved robustness using augmentation and stratified sampling

Identified performance gaps in rare galaxy classes

Established a strong baseline model for future improvement

- Future Improvements

Apply class weighting or oversampling techniques (e.g., SMOTE)

Explore transfer learning (ResNet, VGG)

Experiment with higher-resolution inputs

Improve performance on minority classes

- Technologies Used

Python

TensorFlow / Keras

NumPy

Matplotlib
