# 📊 Diabetic Retinopathy Detection Using Convolutional Neural Networks 

## 📌 Overview
This project implements a **Convolutional Neural Network (CNN)** to detect **diabetic retinopathy (DR)** from fundus retinal images. DR is a leading cause of blindness worldwide, and early detection is critical for effective intervention. Using a subset of a real-world dataset from Kaggle (APTOS 2019), I built a binary classifier to predict whether a patient should be referred for treatment.

## 🎯 Project Goals
- Implement an end-to-end ML pipeline for DR detection.
- Design a custom **CNN architecture** using TensorFlow/Keras.
- Improve generalization and reduce overfitting with **data augmentation** and **dropout regularization**.
- Perform **hyperparameter tuning** to optimize model performance.
- Evaluate model accuracy and classification performance on unseen data.

## 📂 Dataset
| Source | Description |
|--------|-------------|
| A subset of [APTOS 2019 Blindness Detection](https://www.kaggle.com/competitions/aptos2019-blindness-detection) | High-resolution retinal fundus images labeled with severity of diabetic retinopathy. |

- **Task**: Binary classification — *Referral needed* vs. *No referral needed*.
- **Labels**:
  - No/Mild DR → No Referral (Class 0)
  - Moderate/Severe/Proliferative DR → Referral (Class 1)

## 🗂 Files & Notebooks
| File | Description |
|------|-------------|
| `ConvolutionalNeuralNetworkML.ipynb` | Jupyter Notebook containing the full ML pipeline, model design, training, and evaluation steps. |

## 🚀 Implementation Details
### **🔹 Data Preprocessing**
- Image resizing, normalization, and label encoding.
- Data augmentation with image flipping, rotation, zooming.

### **🔹 CNN Model Architecture**
- Multiple convolutional and pooling layers.
- Fully connected dense layers for binary classification.
- Regularization techniques like dropout to combat overfitting.

### **🔹 Hyperparameter Tuning**
- Conducted using **Keras Tuner**.
- Explored different filter sizes, number of layers, dropout rates, and learning rates.
- Tuned models using **Random Search** and **Hyperband**.

### **🔹 Model Training and Evaluation**
- Trained with early stopping to prevent overfitting.
- Evaluated using:
  - Validation Accuracy
  - Confusion Matrix
  - Loss and accuracy curves over epochs.

## 🏆 Performance & Results
The final tuned model achieved strong performance in binary classification, demonstrating the CNN's ability to assist in early diabetic retinopathy screening.  
The project emphasizes real-world healthcare applications, especially in resource-limited settings where AI could significantly reduce clinician workload.
