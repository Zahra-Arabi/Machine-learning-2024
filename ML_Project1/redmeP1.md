📌 Project 1 README (ML_Project1/README.md)

# Machine Learning Project 1 - Customer Churn Prediction

## 📌 Project Overview
This project focuses on **customer churn prediction** using **classification models**. The goal is to predict whether a bank customer will stop using the bank’s services based on demographic and transaction data.

## 📂 Repository Structure

ML_Project1/ │── code/ │ ├── MP1.ipynb # Jupyter Notebook with model implementation │── report/ │ ├── FIS4031_MP1.pdf # Official project report │ ├── ZahraArabi_40007173_FIS4031_MP1.pdf # Student report │── README.md # Project description


## 📊 **Dataset**
- **Dataset Used:** [Bank Churn Dataset](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers)
- **Number of Samples:** 10,127
- **Features:**
  - Customer Age
  - Gender
  - Marital Status
  - Credit Limit
  - Total Transaction Amount
  - Average Utilization Ratio
  - **Target Feature:** `Attrition_Flag` (Indicates if a customer left the bank)

---

## 🛠 **Implementation Steps**
### **1️⃣ Data Preprocessing**
- Load the dataset and check for missing values.
- Convert categorical features to numerical values.
- Normalize and scale numerical features.
- Handle class imbalance using **SMOTE (Synthetic Minority Over-sampling Technique)**.

### **2️⃣ Model Training**
- Train **classification models**:
  - **Random Forest**
  - **Support Vector Machine (SVM)**
- Split the dataset into **Train (70%)**, **Validation (15%)**, and **Test (15%)**.
- Evaluate models using:
  - **Confusion Matrix**
  - **Classification Report (Precision, Recall, F1-score)**
  - **ROC-AUC Score**

### **3️⃣ Model Optimization**
- Compare performance with and without **class balancing**.
- Tune hyperparameters to improve accuracy and reduce **overfitting**.
- Use **Cross-Validation** to ensure model robustness.

---

## 📊 **Results**
| Model | Accuracy | Precision | Recall | F1-score |
|------|------|------|------|------|
| Random Forest (Imbalanced) | 100% | 100% | 100% | 100% |
| Random Forest (Balanced) | 87% | 86% | 85% | 85% |
| SVM (Balanced) | 82% | 81% | 80% | 80% |

📌 **Overfitting Issue:**  
The initial **imbalanced model** achieved 100% accuracy but failed to generalize.  
After **class balancing**, the model achieved a more realistic accuracy of **87%**.

---

## 🚀 **How to Run the Project**
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Zahra-Arabi/Machine-learning-2024.git
   cd Machine-learning-2024/ML_Project1
Open the Jupyter Notebook (MP1.ipynb) in:

Google Colab (Recommended)
Jupyter Notebook
Run all cells and follow the explanations in the notebook.

📌 Google Colab Link:
🔗 Open Notebook **([COLAB MP1](https://colab.research.google.com/drive/1G7SBPrHMCVuey0Pn-m8QP8KHc4OJYp8q?usp=sharing))**

📄 Related Files
📜 Project Report
📑 Student Report



👩‍💻 Author
Name: Zahra Arabi
University: K. N. Toosi University of Technology
Instructor: Dr. Mahdi Aliyari

🚀 Happy Coding! 🎯
