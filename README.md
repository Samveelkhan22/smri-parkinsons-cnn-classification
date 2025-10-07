# 🧠 sMRI Parkinson's Disease Classification using 3D CNN

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-1.9%2B-orange)
![MONAI](https://img.shields.io/badge/MONAI-0.7%2B-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

A deep learning pipeline for classifying **Parkinson's Disease (PD)** vs. **Healthy Controls (HC)** using structural MRI (sMRI) scans and a 3D DenseNet model.

---

## 🚀 Features

- ✅ 3D MRI preprocessing & augmentation using `TorchIO`
- ✅ 2D & 3D dataset loaders with weighted sampling
- ✅ 3D DenseNet121 model with custom classifier
- ✅ Training with class imbalance handling & early stopping
- ✅ Evaluation metrics: AUC, Accuracy, Precision, Recall, F1-Score

---

## 📊 Dataset

- **Classes:** Parkinson's Disease (1) vs. Healthy Control (0)
- **Preprocessing:** Min-Max normalization, cropping, resizing to `(128, 128, 128)`
- **Augmentation:** Random affine, elastic deformation, noise

---

## 🧩 Model Architecture

- **Backbone:** `MONAI 3D DenseNet121`
- **Input:** `1 x 128 x 128 x 128`
- **Output:** Binary classification (PD vs. HC)
- **Custom Classifier:** Dropout (0.5) + Linear(1024 → 1)

---

## 📈 Results

| Metric       | Value  |
|--------------|--------|
| Accuracy     | 76.62% |
| Precision    | 87.18% |
| Recall       | 82.93% |
| F1-Score     | 85.00% |
| ROC AUC      | 80.09% |

---

## 📦 Dependencies

- torch
- monai
- torchio
- nibabel
- scipy
- scikit-learn
- pandas
- matplotlib

  
