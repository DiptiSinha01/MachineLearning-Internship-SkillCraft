# 🐶🐱 Cat vs Dog Classification with SVM - SkillCraft Internship (Task 3)

This project is part of **Task 3** from the **SkillCraft Technology Internship Program**, where the goal was to classify images of cats and dogs using **Support Vector Machines (SVM)** — *without using deep learning classification models*.

---

## 📌 Project Summary

* **Model**: Support Vector Machine (SVM)
* **Dataset**: Dogs vs Cats dataset (Microsoft Research)
* **Input**: 64x64 grayscale images (flattened)
* **Preprocessing**:

  * Resizing
  * Grayscale conversion
  * Normalization
  * PCA for dimensionality reduction
* **Initial Accuracy**: \~65%
* **Final Accuracy**: **\~71%** (after optimization)

---

## 📁 Dataset Setup

The dataset is sourced from Microsoft Research. You can use the following steps to set it up:

### ✅ Step 1: Download Dataset

Download the original Dogs vs Cats dataset from the official Microsoft Research page:

🔗 [Download from Microsoft](https://www.microsoft.com/en-us/download/details.aspx?id=54765)

Choose `dogs-vs-cats.zip` and manually download it.

### 📄 Step 2: Upload to Google Drive

1. Upload the `dogs-vs-cats.zip` file to your Google Drive (e.g., `My Drive`)
2. Update the `zip_path` in the notebook to match the uploaded location

```python
zip_path = '/content/drive/MyDrive/cats_dogs_dataset.zip'
```

### 📂 Step 3: Extract and Use

The notebook will unzip and extract the dataset. If the dataset doesn't include subfolders (`Cat`, `Dog`), split images manually or via code after extraction.

---

## 📊 Evaluation Metrics

The model was evaluated on:

* **Accuracy**
* **Classification Report** (Precision, Recall, F1)
* **Confusion Matrix**

### Confusion Matrix (Final Model \~71% accuracy)

<img width="659" height="539" alt="image" src="https://github.com/user-attachments/assets/0b327bb0-1ce0-42e6-b202-d05f3261c6e9" />


---

## 🚀 Improvements Made

* Replaced hardcoded paths with configurable variables
* Added PCA to reduce noise in high-dimension pixel data
* Tuned SVM hyperparameters (`C`, `gamma`, kernel)
* Modularized loading and preprocessing pipeline

---

## 🧐 Future Work

* Extract features using pretrained CNNs (like MobileNetV2)
* Compare performance with deep learning models (CNNs, ResNet)
* Expand to multi-class classification (other animal categories)

---

## 🤝 Credits

* **Internship**: SkillCraft Technology, Task 3
* **Notebook & Code**: Developed by Dipti Sinha

---

## 🔗 Links

* 📓 https://colab.research.google.com/drive/1pXpX_1ENfcsgNPtc5a3CwmvnSnzoZ2K_?usp=sharing
* 📁 [Dataset (Microsoft Download Link)](https://www.microsoft.com/en-us/download/details.aspx?id=54765)

---

> Have questions or suggestions? Feel free to connect!
