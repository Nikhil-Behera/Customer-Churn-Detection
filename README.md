# 📊 Telco Customer Churn Prediction

A Machine Learning project that analyzes and predicts **customer churn** for a telecommunications company using multiple classification algorithms. The project leverages the Telco Customer Churn dataset to identify patterns in customer behavior and predict which customers are likely to churn.

---

## 🎯 Objective

The goal of this project is to build and compare various machine learning models to predict whether a telecom customer will churn (leave the service) based on their demographic information, account details, and service usage patterns.

---

## 📁 Project Structure

```
ML_Mini_Project/
├── ML_mini_prj_2nd.ipynb      # Main Jupyter Notebook with full analysis
├── Telco_customer_churn.xlsx   # Dataset
├── LICENSE                     # MIT License
└── README.md                   # Project documentation
```

---

## 📋 Dataset Overview

- **Source**: Telco Customer Churn Dataset
- **Samples**: 7,043 customers
- **Features**: 33 columns
- **Target Variable**: `Churn Value` (Binary: 0 = No Churn, 1 = Churn)
- **Churn Rate**: ~26.5%

### Key Features

| Category           | Features                                                                                           |
|---------------------|-----------------------------------------------------------------------------------------------------|
| **Demographics**    | Gender, Senior Citizen, Partner, Dependents                                                        |
| **Account Info**    | Tenure Months, Contract, Paperless Billing, Payment Method, Monthly Charges, Total Charges          |
| **Services**        | Phone Service, Multiple Lines, Internet Service, Online Security, Online Backup, Device Protection  |
| **Streaming**       | Tech Support, Streaming TV, Streaming Movies                                                       |
| **Churn Details**   | Churn Label, Churn Value, Churn Score, CLTV, Churn Reason                                          |

---

## 🔬 Methodology

### 1. Data Preprocessing
- **Loading**: Data loaded from Excel (`.xlsx`) format using `pandas` and `openpyxl`
- **Missing Values**: Handled using `SimpleImputer` from scikit-learn
- **Encoding**: Categorical features encoded using `LabelEncoder`
- **Scaling**: Features standardized using `StandardScaler`
- **Splitting**: Train/test split via `train_test_split`

### 2. Exploratory Data Analysis (EDA)
- Data type analysis and missing value detection
- Target distribution visualization (Churn vs No Churn)
- Feature correlation analysis
- Visual exploration using `matplotlib` and `seaborn`

### 3. Models Implemented

| Model                          | Description                                   |
|--------------------------------|-----------------------------------------------|
| **SVM (Linear Kernel)**        | Support Vector Machine with linear kernel      |
| **SVM (Polynomial Kernel)**    | Support Vector Machine with polynomial kernel  |
| **SVM (Sigmoid Kernel)**       | Support Vector Machine with sigmoid kernel     |
| **SVM (RBF Kernel)**           | Support Vector Machine with RBF kernel         |
| **KNN**                        | K-Nearest Neighbors Classifier                 |
| **Logistic Regression**        | Logistic Regression Classifier                 |

### 4. Evaluation Metrics
- **Accuracy Score**
- **ROC-AUC Score**
- **Classification Report** (Precision, Recall, F1-Score)
- **Confusion Matrix**
- **ROC Curves** (individual per model)
- **Cross-Validation Scores**
- **PCA Visualizations**

---

## 📈 Results & Visualizations

The project includes comprehensive comparative analysis:

- **Model Accuracy Comparison** — Bar chart comparing accuracy across all 6 models
- **ROC-AUC Score Comparison** — Bar chart comparing AUC scores across all models
- **Individual ROC Curves** — Per-model ROC curves with AUC annotations
- **Confusion Matrices** — Visual confusion matrix for each classifier
- **PCA Plots** — Dimensionality reduction for data visualization

---

## 🛠️ Tech Stack

| Tool / Library     | Purpose                                   |
|--------------------|-------------------------------------------|
| **Python 3.13**    | Programming Language                      |
| **pandas**         | Data manipulation and analysis            |
| **NumPy**          | Numerical computing                       |
| **matplotlib**     | Data visualization                        |
| **seaborn**        | Statistical data visualization            |
| **scikit-learn**   | Machine learning models and utilities     |
| **openpyxl**       | Reading Excel files                       |
| **Jupyter Notebook** | Interactive development environment     |

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.x installed, then install the required packages:

```bash
pip install pandas openpyxl scikit-learn matplotlib seaborn numpy
```

### Running the Project

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Nikhil-Behera/Customer-Churn-Detection.git
   cd Customer-Churn-Detection
   ```

2. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook ML_mini_prj_2nd.ipynb
   ```

3. **Run all cells** sequentially to reproduce the full analysis.

---

## 📌 Key Findings

- The dataset exhibits a **class imbalance** with approximately 73.5% non-churn and 26.5% churn customers
- Multiple SVM kernel variants were tested to find the optimal decision boundary
- Model performance was evaluated using both accuracy and AUC metrics for a comprehensive assessment
- Comparative visualizations help identify the best-performing model for churn prediction

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Nikhil Behera**

- GitHub: [@Nikhil-Behera](https://github.com/Nikhil-Behera)
