📌 Project 3 README (ML_Project3/README.md)

# Machine Learning Project 3 - PID and Fuzzy Logic Control Systems

## 📌 Project Overview
This project compares **PID controllers** and **Fuzzy Logic controllers** for controlling **nonlinear dynamic systems**. The aim is to analyze different tuning techniques, evaluate system stability, and optimize control performance.

## 📂 Repository Structure

ML_Project3/ │── code/ │ ├── MP3.ipynb # Jupyter Notebook with model implementation │── report/ │ ├── FIS4031_MP3.pdf # Official project report │ ├── ZahraArabi_40007173_FIS4031_MP3.pdf # Student report │── README.md # Project description


## 🛠 **Implementation Steps**
### **1️⃣ PID Controller Design**
- Implemented a **Ziegler-Nichols tuned PID controller**.
- Designed an **auto-tuned PID controller (CHR method)**.
- Evaluated **overshoot, settling time, and response characteristics**.

### **2️⃣ Fuzzy Logic Controller Design**
- Created a **fuzzy inference system** for control.
- Defined **membership functions** for:
  - **X Position (Left, Target, Right)**
  - **Angle (Negative, Small, Target, Large)**
  - **Steering (SharpLeft, Left, Zero, Right, SharpRight)**
- Applied **Mamdani inference** for decision-making.

### **3️⃣ Performance Comparison**
- Compared **PID and fuzzy controllers** based on:
  - **Rise Time, Settling Time, Overshoot**
  - **Integral Absolute Error (IAE)**
  - **Integral Time-Weighted Absolute Error (ITAE)**
  - **Stability & Robustness against noise**

---

## 📊 **Results**
| Controller | Overshoot (%) | Settling Time (s) | IAE | ITAE |
|------|------|------|------|------|
| Ziegler-Nichols PID | 28.38 | 0.721 | 0.767 | 0.447 |
| Fuzzy PID | 0.00 | 7.252 | 2.034 | 4.035 |
| Auto-tuned PID | 0.00 | 3.709 | 0.837 | 0.708 |

📌 **Key Observations:**
- **Ziegler-Nichols PID** is **fast but unstable** with **high overshoot**.
- **Fuzzy PID** is **stable but slow**, ideal for systems requiring **smooth control**.
- **Auto-tuned PID (CHR method)** balances **speed and stability**, making it **optimal for industrial applications**.

---

## 🚗 **Car Parking Fuzzy Control System**
- Simulated **autonomous car parking** using **fuzzy logic**.
- Defined control rules based on **X position & angle**.
- Evaluated **mean & max error**:
  - **Mean Position Error:** 1.2946
  - **Max Position Error:** 2.1887
  - **Mean Angle Error:** 0.7517
  - **Max Angle Error:** 2.9544

📌 **Key Findings:**
- The **fuzzy system performs well for standard parking scenarios**.
- In **complex scenarios**, additional **fuzzy rules** are needed for higher precision.

---

## 🏭 **Industrial System Control Analysis**
### **1️⃣ Ball and Beam System**
- Simulated **ball position control on a beam**.
- Modeled **neural network-based system identification**.
- **RMSE Error:** **0.0468**
- **MAE Error:** **0.0362**
📌 **Key Takeaways:**
- The **model successfully learns system behavior**.
- **Neural networks can approximate nonlinear dynamics effectively**.

### **2️⃣ Steam Generator Control**
- Modeled a **steam generator system** for industrial control.
- **Regression-based system identification** with **ML models**.
- **Best-performing model (Excess Oxygen output):**
  - **RMSE:** **3.65**
  - **R² Score:** **0.658**

📌 **Key Observations:**
- The **oxygen control model performed best**, explaining **65.8% of variance**.
- The **water level control model had the lowest accuracy**, requiring **further optimization**.

---

## 📈 **Adaptive Fuzzy System for Nonlinear Function Approximation**
- Modeled **Takagi-Sugeno-Kang (TSK) Fuzzy Systems**.
- Trained **Adaptive Neuro-Fuzzy Inference System (ANFIS)**.
- Compared **Gaussian Process Regression (GPR) vs. ANFIS**:
  - **GPR MSE:** **702.74**
  - **ANFIS MSE:** **1115.55**
  - **GPR R² Score:** **0.349**
  - **ANFIS R² Score:** **-0.032**

📌 **Conclusion:**
- **Gaussian Process Regression outperformed ANFIS** in this dataset.
- **ANFIS struggled with learning the function due to data limitations**.
- **Regularization & larger datasets needed** for ANFIS to generalize well.

---

## 🚀 **How to Run the Project**
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Zahra-Arabi/Machine-learning-2024.git
   cd Machine-learning-2024/ML_Project3


Open the Jupyter Notebook (MP3.ipynb) in:

Google Colab (Recommended)
Jupyter Notebook
Run all cells and follow the explanations in the notebook.

📌 Google Colab Link:
🔗 Open Notebook (Replace with actual link)

📄 Related Files
📜 Project Report
📑 Student Report

🔗 Additional Resources
📜 Main Repository
📑 ML Final Project

👩‍💻 Author
Name: Zahra Arabi
University: K. N. Toosi University of Technology
Instructor: Dr. Mahdi Aliyari

🚀 Happy Coding! 🎯
