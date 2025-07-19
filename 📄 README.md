# 🤟 Real-Time Sign Language Recognition using MATLAB

This project implements a real-time sign language recognition system using MATLAB. It trains a classifier to recognize American Sign Language (ASL) alphabets using HOG (Histogram of Oriented Gradients) features and a multi-class SVM model.

---

## 📁 Project Structure

SignLanguageRecognition-MATLAB/
├── train_model.m # Script to train the SVM classifier
├── predict_model.m # Script to evaluate and test predictions
├── aslAZClassifier_HOG.mat # Trained model file (generated after training)
├── .gitignore # Git exclusions for MATLAB
├── README.md # Project documentation
└── DATASET/ # Folder containing ASL alphabet images (not uploaded)

---

## 🚀 How It Works

1. **Training (`train_model.m`)**:
   - Loads images from the dataset.
   - Extracts HOG features.
   - Trains a multi-class linear SVM classifier.
   - Saves the model as `aslAZClassifier_HOG.mat`.

2. **Prediction (`predict_model.m`)**:
   - Loads the trained model.
   - Re-evaluates accuracy on the validation set.
   - Predicts random validation samples.
   - Displays confusion matrix and sample predictions.

---

## 📦 Requirements

- MATLAB R2021a or later
- Image Processing Toolbox
- Statistics and Machine Learning Toolbox

---

## 📂 Dataset

Dataset should be structured like this inside the `DATASET/` folder:

DATASET/
├── A/
│ ├── img1.jpg
│ └── ...
├── B/
│ ├── img1.jpg
│ └── ...
...

> Each folder should be named after the ASL letter it represents (`A`, `B`, ..., `Z`).

---

## 🛠️ How to Run

### 1. Train the Model
```matlab
>> run('train_model.m')
>> run('predict_model.m')
📊 Output
.Confusion matrix for validation accuracy
.Sample predictions with true and predicted labels

🙋‍♂️ Author
Created by Akshat Pal
