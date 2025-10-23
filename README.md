# Regression-Using-ANN

Perfect ✅ — here’s a clean, professional **README.md** file for your project based on
the **Folds5x2_pp.xlsx (Combined Cycle Power Plant)** dataset and your **ANN regression code** from that GitHub example.

You can copy this straight into your project folder as `README.md`.

---

# 🔥 Artificial Neural Network – Power Plant Energy Output Prediction

## 📘 Project Overview

This project demonstrates how to build a simple **Artificial Neural Network (ANN)** for a **regression problem** using Python, TensorFlow/Keras, and the **Combined Cycle Power Plant (CCPP)** dataset.

The model predicts the **net electrical energy output (PE)** of a power plant based on four environmental factors:

* **AT** – Ambient Temperature (°C)
* **V** – Exhaust Vacuum (cm Hg)
* **AP** – Ambient Pressure (millibar)
* **RH** – Relative Humidity (%)

---

## 🧠 Problem Statement

Predict the **net hourly electrical energy output (PE)** of a combined cycle power plant using sensor data collected over six years.

This is a **supervised regression problem**.

---

## 📊 Dataset Information

**Dataset name:** `Folds5x2_pp.xlsx`
**Source:** [UCI Machine Learning Repository – Combined Cycle Power Plant Dataset](https://archive.ics.uci.edu/dataset/294/combined+cycle+power+plant)

**Description:**

* Contains 9,568 data points.
* Each record consists of 4 features and 1 target variable.
* Data collected from a combined cycle power plant operating under different conditions.

| Column | Description                           | Unit     |
| ------ | ------------------------------------- | -------- |
| AT     | Ambient Temperature                   | °C       |
| V      | Exhaust Vacuum                        | cm Hg    |
| AP     | Ambient Pressure                      | millibar |
| RH     | Relative Humidity                     | %        |
| PE     | Net Electrical Energy Output (Target) | MW       |

---

## ⚙️ Technologies Used

* **Python 3.8+**
* **TensorFlow / Keras**
* **pandas**
* **NumPy**
* **Matplotlib**
* **scikit-learn**

---

## 🚀 How to Run the Project

### 1. Clone or Download the Repository

```bash
git clone https://github.com/<your-username>/ANN-Beginner-Projects.git
cd ANN-Beginner-Projects/Regression-Exercise
```

### 2. Install Dependencies

```bash
pip install tensorflow pandas numpy matplotlib scikit-learn openpyxl
```

### 3. Download the Dataset

You can download the dataset directly from UCI:

```
https://archive.ics.uci.edu/ml/machine-learning-databases/00294/CCPP.zip
```

Extract `Folds5x2_pp.xlsx` into your project folder.

Alternatively, download it automatically in Jupyter:

```python
!wget https://archive.ics.uci.edu/ml/machine-learning-databases/00294/CCPP.zip
!unzip CCPP.zip
```

### 4. Run the Code

In Jupyter Notebook or a Python IDE:

```bash
python artificial_neural_network.py
```

or inside a notebook cell:

```python
%run artificial_neural_network.py
```

---

## 🧩 Code Workflow

1. **Load Dataset**

   ```python
   dataset = pd.read_excel('Folds5x2_pp.xlsx')
   ```
2. **Split into features and target**

   ```python
   X = dataset.iloc[:, :-1].values
   y = dataset.iloc[:, -1].values
   ```
3. **Preprocess Data (Scaling + Splitting)**
4. **Build ANN Model (Keras Sequential API)**
5. **Train Model**
6. **Evaluate Model Performance (MAE, MSE, R²)**
7. **Visualize Loss Curve**

---

## 📈 Example Model Architecture

| Layer | Type  | Units | Activation                 |
| ----- | ----- | ----- | -------------------------- |
| 1     | Dense | 6     | ReLU                       |
| 2     | Dense | 6     | ReLU                       |
| 3     | Dense | 1     | Linear (Regression Output) |

---

## 📊 Sample Results

| Metric              | Value |
| ------------------- | ----- |
| Training Loss (MSE) | ~20   |
| Test Loss (MSE)     | ~22   |
| R² Score            | ~0.93 |

*Results may vary slightly depending on training epochs and random seed.*

---

## 📘 References

* UCI Machine Learning Repository: [Combined Cycle Power Plant Dataset](https://archive.ics.uci.edu/dataset/294/combined+cycle+power+plant)
* TensorFlow Documentation: [https://www.tensorflow.org](https://www.tensorflow.org)
* Original Project Inspiration: [PritiG1/ANN-Beginner-Projects](https://github.com/PritiG1/ANN-Beginner-Projects)

---

## 🧩 Author

**Your Name**
📧 [[your.email@example.com](mailto:your.email@example.com)]
💻 [GitHub Profile](https://github.com/your-username)

---

Would you like me to include a **code example** section inside the README (so it shows a small snippet of the ANN model architecture and training code)?
