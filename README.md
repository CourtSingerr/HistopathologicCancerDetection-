# CNN Cancer Detection (Kaggle Mini-Project)

This repository contains code and documentation for a Histopathologic Cancer Detection project, aiming to classify small histopathology image patches as cancerous or non-cancerous using convolutional neural networks (CNNs). The data comes from the Histopathologic Cancer Detection Kaggle competition, where each 96×96 RGB image patch shows a section of lymph node tissue.

## Project Overview

The goal is to build a reliable CNN-based model to detect metastatic cancer in histopathology images. This involves:
-	Preprocessing & EDA: Cleaning, normalizing, and exploring large-scale image data.
-	Model Development: Training multiple CNN architectures (Baseline, Deeper Model, Advanced Model) and comparing their performance.
-	Hyperparameter Tuning: Systematically searching for optimal filter sizes, dropout rates, dense layer units, and learning rates using Keras Tuner.
-	Evaluation & Analysis: Using metrics like Accuracy, AUC, Confusion Matrix, and Classification Report to assess model performance on validation and test data.

 ## Data Description
-	Dataset Scale: ~220,000 labeled training images, similarly large test set without labels.
- Image Format: TIFF files of size 96 × 96 (RGB).
-	Labels: Binary (1 for cancerous, 0 for non-cancerous).
-	Directories:
-	train/ folder with labeled images.
-	test/ folder with unlabeled images.
-	train_labels.csv mapping image id to a label.

This dataset is available through Kaggle. See the competition’s Data page for details.

## Key Results
- Best Model: Achieved ~92.5% validation accuracy and an AUC of ~0.978.
- Confusion Matrix: About 10% false negatives on the validation set, implying room for further improvement in catching subtle cancer cases.
- Kaggle Score:
- Public LB Score: 0.6440
- Private LB Score: 0.5313


