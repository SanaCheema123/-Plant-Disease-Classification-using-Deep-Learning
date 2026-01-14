# 🌱 Plant Disease Classification using Deep Learning

This repository contains an end-to-end deep learning pipeline for **plant disease classification** using a **pretrained EfficientNetB0** model. The project covers dataset preparation, exploratory data analysis (EDA), model training, and comprehensive evaluation.

## 📌 Project Overview

Plant diseases pose a major threat to agricultural productivity. This project applies **computer vision and transfer learning** to automatically classify plant leaf images into disease categories.

## 📂 Dataset

- **Source:** Kaggle – Plant Disease Recognition Dataset  
- **Access Method:** KaggleHub API  
- **Structure (resolved):**


Train/Train/
Validation/Validation/
Test/Test/

- Each directory contains multiple disease class folders (e.g., `Powdery`, `Rust`, `Healthy`).

## 🔍 Exploratory Data Analysis (EDA)

The following EDA steps were performed:
- Class-wise image count analysis
- Visualization of class distribution
- Inspection of random sample images
- Verification of image dimensions and format

## 🧠 Model Architecture

- **Backbone:** EfficientNetB0 (pretrained on ImageNet)
- **Modifications:**
- Global Average Pooling
- Dropout (0.3)
- Fully Connected Softmax Layer
- **Loss Function:** Categorical Cross-Entropy
- **Optimizer:** Adam


## 🏋️ Model Training

- **Image Size:** 224 × 224  
- **Batch Size:** 32  
- **Epochs:** 5  
- **Data Augmentation:**
- Random horizontal flip
- Random rotation
- Random zoom

Training and validation accuracy and loss were monitored across all epochs.

## 📊 Evaluation Metrics

The model was evaluated on an unseen test set using the following metrics:

- Accuracy
- Precision (weighted)
- Recall (weighted)
- F1-score (weighted)
- Confusion Matrix
- Test Loss

Metrics were computed using **scikit-learn** for reliable multi-class evaluation.



## 📈 Results

- Stable convergence observed during training
- High classification performance across disease classes
- Confusion matrix analysis provided insights into misclassification patterns

Detailed metrics were exported to a CSV file for reporting purposes.

## 🛠 Technologies Used

- Python
- TensorFlow / Keras
- scikit-learn
- NumPy, Pandas
- Matplotlib
- Google Colab
- KaggleHub API

## 🚀 Future Improvements

- Fine-tuning EfficientNet layers
- Comparison with ResNet50 and MobileNetV2
- Class imbalance handling
- Explainable AI (Grad-CAM)
- Deployment as a web or mobile application

## 🤝 Contributions

Contributions, suggestions, and collaborations are welcome.  
Feel free to open an issue or submit a pull request.

## 📄 License

This project is intended for **academic and research purposes**.

