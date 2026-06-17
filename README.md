<p align="center"> <!-- Deep Learning --> <img src="https://img.shields.io/badge/Deep%20Learning-CNNs%20%7C%20Transformers-orange?style=for-the-badge" /> <img src="https://img.shields.io/badge/Models-VGG16%20%7C%20ResNet50%20%7C%20DenseNet121-blue?style=for-the-badge" /> <!-- Transformers --> <img src="https://img.shields.io/badge/Transformers-ViT%20%7C%20Hybrid-green?style=for-the-badge" /> <!-- Frameworks --> <img src="https://img.shields.io/badge/Framework-TensorFlow%20%2F%20Keras-orange?style=for-the-badge" /> <!-- Libraries --> <img src="https://img.shields.io/badge/Libraries-NumPy%20%7C%20Pandas%20%7C%20OpenCV-yellow?style=for-the-badge" /> <img src="https://img.shields.io/badge/Visualization-Matplotlib%20%7C%20Seaborn%20%7C%20Plotly-lightblue?style=for-the-badge" /> <!-- ML Tasks --> <img src="https://img.shields.io/badge/Tasks-MRI%20Processing%20%7C%20EDA%20%7C%20Augmentation-purple?style=for-the-badge" /> <img src="https://img.shields.io/badge/Evaluation-Accuracy%20%7C%20F1%20%7C%20AUC%20%7C%20ROC-red?style=for-the-badge" /> <img src="https://img.shields.io/badge/Training-GPU%20Accelerated-brightgreen?style=for-the-badge" /> </p>

🧠 Brain Tumor Detection Using CNNs
A Comparative Study on MRI Image Classification








🚀 Project Overview

This project presents a comprehensive comparison of CNN models (VGG16, ResNet50, DenseNet121)  for multi-class brain tumor detection using MRI images.
Models were trained under identical conditions and evaluated using accuracy, F1-score, ROC-AUC, confusion matrices, and loss/accuracy curves to determine which architecture performs best for medical imaging tasks.

Dataset includes 4 classes:

🟦 Glioma

🟥 Meningioma

🟩 Pituitary

⬜ No Tumor

📂 Dataset

Kaggle Brain Tumor MRI Dataset
Training: 4571 images
Validation: 1141 images
Testing: 1311 images

Balanced class distribution (verified using treemaps & histograms).

🛠️ Technologies Used

Deep Learning: VGG16, ResNet50, DenseNet121, Transformers
Frameworks: TensorFlow / Keras
EDA & Visualization: Matplotlib, Seaborn, Plotly
Libraries: NumPy, Pandas, OpenCV, PIL
Evaluation: AUC-ROC, F1-score, Precision/Recall, Confusion Matrix

🔧 Model Training Pipeline

Import libraries

Data loading & preprocessing (224×224, grayscale→RGB, normalization)

Augmentation (rotation, zoom, flips)

Build CNN & Transformer models

Train using EarlyStopping + Checkpointing

Evaluate on test set

Generate plots & metrics

📊 Results Summary
Model	Test Accuracy	F1-Score	ROC-AUC
DenseNet121	⭐ 0.8658	0.83+	0.94+
VGG16	0.7918	0.7778	0.9282
ResNet50	0.6491	0.6290	0.8358

➡️ DenseNet121 achieved the highest performance overall.

📈 Visualizations

This repository includes the following plots:

✔ Training vs Validation Accuracy
✔ Training vs Validation Loss
✔ Class-wise ROC Curves
✔ Confusion Matrix
✔ Sample MRI Heatmaps
✔ Dataset EDA (image counts, pixel intensity stats, treemaps)
