📌 Project 2 README (ML_Project2/README.md)

# Machine Learning Project 2 - Neural Network Analysis & Optimization

## 📌 Project Overview
This project focuses on **analyzing and optimizing artificial neural networks**. The primary objective is to experiment with different architectures, activation functions, and optimization techniques to improve model accuracy and robustness.

## 📂 Repository Structure
ML_Project2/ │── code/ │ ├── MP2.ipynb # Jupyter Notebook with model implementation │── report/ │ ├── FIS4031_MP2.pdf # Official project report │ ├── ZahraArabi_40007173_FIS4031_MP2.pdf # Student report │── README.md # Project description


## 📊 **Dataset**
- **Dataset Used:** [Telecommunications Customer Segmentation Dataset](https://www.kaggle.com/datasets/aslkuscu/telecust1000t)
- **Number of Samples:** 1000
- **Features:**
  - Age, Marital Status, Income
  - Service Usage Patterns
  - **Target Feature:** `custcat` (Customer Category: Basic, Electronic, Advanced, Premium)

---

## 🛠 **Implementation Steps**
### **1️⃣ Data Preprocessing**
- Load the dataset and handle missing values.
- Convert categorical features to numerical values.
- Normalize the dataset using **MinMaxScaler**.
- Split the dataset into **Train (60%)**, **Validation (20%)**, and **Test (20%)**.

### **2️⃣ Model Training**
- Train **Multi-Layer Perceptron (MLP) models** with different architectures:
  - **Model 1:** Single hidden layer with 32 neurons.
  - **Model 2:** Two hidden layers (32 and 16 neurons).
- Compare different activation functions:
  - **ReLU, Sigmoid, Tanh**
- Optimize using different techniques:
  - **Batch Normalization**
  - **Dropout**
  - **L2 Regularization**
- Test different optimizers:
  - **SGD, Adam, RMSprop**

### **3️⃣ Model Evaluation**
- Assess model performance using:
  - **Accuracy, Precision, Recall, F1-score**
  - **Confusion Matrix**
  - **Loss curves and validation metrics**
- Compare performance before and after **regularization techniques**.

---

## 📊 **Results**
| Model | Accuracy | Validation Accuracy |
|------|------|------|
| Baseline MLP | 78% | 72% |
| MLP + Batch Normalization | 85% | 83% |
| MLP + Dropout | 81% | 79% |
| MLP + L2 Regularization | 83% | 80% |

📌 **Best Model:** MLP with **Batch Normalization**  
📌 **Main Improvement:** Prevented **overfitting** and improved **generalization**.

---

## 🚀 **How to Run the Project**
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Zahra-Arabi/Machine-learning-2024.git
   cd Machine-learning-2024/ML_Project2

Open the Jupyter Notebook (MP2.ipynb) in:

Google Colab (Recommended)
Jupyter Notebook
Run all cells and follow the explanations in the notebook.

📌 Google Colab Link:
🔗 Open Notebook (Replace with actual link)

📄 Related Files
📜 Project Report
📑 Student Report

👩‍💻 Author
Name: Zahra Arabi
University: K. N. Toosi University of Technology
Instructor: Dr. Mahdi Aliyari

🚀 Happy Coding! 🎯

