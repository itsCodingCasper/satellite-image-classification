# 🛰️ Satellite Land Cover Classification using ResNet50

A deep learning project that classifies satellite images into **10 land-cover categories** using **Transfer Learning with ResNet50** and the **EuroSAT** dataset.

This project demonstrates how pretrained convolutional neural networks can be adapted for remote sensing tasks with minimal training while achieving high classification performance.

---

## 📌 Project Overview

Satellite imagery plays an important role in environmental monitoring, agriculture, urban planning, and disaster management. In this project, a pretrained **ResNet50** model is fine-tuned to classify satellite images into different land-cover classes.

Instead of training a convolutional neural network from scratch, this project uses **transfer learning**, allowing the model to leverage features learned from millions of natural images and adapt them to satellite imagery.

---

## 📂 Dataset

**Dataset:** EuroSAT RGB

The EuroSAT dataset contains approximately **27,000 RGB satellite images** collected from Sentinel-2 satellites.

The dataset consists of **10 land-cover classes:**

- Annual Crop
- Forest
- Herbaceous Vegetation
- Highway
- Industrial
- Pasture
- Permanent Crop
- Residential
- River
- Sea/Lake

---

## 🧠 Model Architecture

- Pretrained ResNet50
- Transfer Learning
- Final fully connected layer replaced with 10 output classes
- CrossEntropy Loss
- Adam Optimizer

---

## ⚙️ Workflow

1. Load EuroSAT dataset
2. Apply image preprocessing
   - Resize to 224×224
   - Normalization
   - Data augmentation
3. Split dataset into
   - Training
   - Validation
   - Test
4. Load pretrained ResNet50
5. Freeze feature extraction layers
6. Train classification head
7. Evaluate model performance

---

## 📊 Results

The model was evaluated using:

- Validation Accuracy
- Test Accuracy
- Confusion Matrix
- Classification Report
- Precision
- Recall
- F1-score

Example:

| Metric | Value |
|---------|--------|
| Validation Accuracy |  95.63% |
| Test Accuracy | 95% |

---

## 📸 Sample Outputs

- Validation Accuracy
<img width="319" height="92" alt="image" src="https://github.com/user-attachments/assets/885630ff-028d-439b-8638-5e9edab2f1d7" />

Classification Report
<img width="442" height="232" alt="image" src="https://github.com/user-attachments/assets/8e9047d2-62fb-4c62-84cc-6ebbf690d650" />

- Confusion Matrix
<img width="855" height="768" alt="image" src="https://github.com/user-attachments/assets/f8a37dfc-cf7a-4484-b713-f40e4225f5e6" />






---

## 🛠️ Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

---

## 📁 Repository Structure

```
satellite-land-cover-classification/

│── notebook/
│     Satellite_Image_Classifier.ipynb

│── images/

│── README.md

│── requirements.txt

│── LICENSE
```

---

## 🚀 Future Improvements

- Fine-tune the entire ResNet50 network ✓
- Use multispectral Sentinel-2 bands ✓
- Apply the classifier to real satellite imagery ✓
- Detect land-cover changes between different years ✓
- Build a complete deforestation detection pipeline

---

## 📖 References

- EuroSAT Dataset
- PyTorch Documentation
- Torchvision Models
- ResNet50 Paper

---

## 👤 Author

**Arpita**

B.Tech Computer Science Engineering
Computer Vision • Machine Learning • Remote Sensing
