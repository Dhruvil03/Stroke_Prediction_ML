# 🧠 Stroke Prediction using Machine Learning

This project applies machine learning techniques to predict the likelihood of a patient experiencing a stroke based on key health indicators. The goal is to use data-driven analysis to identify high-risk individuals early and improve preventive healthcare decisions.

---

## 📂 Project Structure

```

Stroke_Prediction_ML/
├── Stroke_detection.ipynb                # Main notebook (EDA, preprocessing, modeling)
├── healthcare-dataset-stroke-data.csv    # Dataset used for training and evaluation
├── Stroke_Prediction.pdf                 # Report summarizing findings
└── README.md                             # Project documentation

````

---

## 📊 Dataset Overview

The dataset contains patient information with the following features:

- **gender**
- **age**
- **hypertension**
- **heart_disease**
- **ever_married**
- **work_type**
- **Residence_type**
- **avg_glucose_level**
- **bmi**
- **smoking_status**
- **stroke** *(target variable: 1 = stroke, 0 = no stroke)*

⚠️ **Imbalanced dataset:** Stroke cases are rare, so special care is needed during model training and evaluation.

---

## 🧪 Workflow Summary

All exploration and modeling steps are implemented in **`Stroke_detection.ipynb`**.

### **1. Data Exploration (EDA)**  
- Visualizing feature distributions  
- Examining correlations  
- Understanding relationships between features and stroke occurrence  

### **2. Data Preprocessing**  
- Handling missing values (e.g., BMI)  
- Encoding categorical variables  
- Scaling numerical features  
- Splitting into training and testing sets  

### **3. Machine Learning Models**  
Models tested include (depending on notebook implementation):
- Logistic Regression  
- Random Forest Classifier  
- Gradient Boosting / other tree-based models  

### **4. Evaluation Metrics**  
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

Emphasis is placed on **recall**, since detecting stroke-prone patients is crucial.

---

## 🛠️ Installation & Setup

### **1. Clone this repository**
```bash
git clone https://github.com/Dhruvil03/Stroke_Prediction_ML.git
cd Stroke_Prediction_ML
````

### **2. (Optional) Create a virtual environment**

```bash
python -m venv venv
source venv/bin/activate    # Windows: venv\Scripts\activate
```

### **3. Install dependencies**

If no `requirements.txt` is provided, install manually:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn jupyter
```

### **4. Run the notebook**

```bash
jupyter notebook
```

Open **`Stroke_detection.ipynb`** and run all cells.

---

## 📈 Results Overview

This project evaluates multiple ML models and compares their performance on stroke prediction.
You can update this section with actual metrics from your notebook (accuracy, F1-score, ROC-AUC, etc.).

---

## 🚀 Future Improvements

* Add hyperparameter tuning
* Test advanced models (XGBoost, LightGBM)
* Apply SMOTE or other resampling for class imbalance
* Deploy as a REST API using Flask/FastAPI
* Build a simple UI for predictions

---

## 📄 Report

A detailed summary of the project and results can be found in:

📘 **Stroke_Prediction.pdf**

---

## 🤝 Contributing

Feel free to fork this repository, explore the notebook, and open a pull request if you'd like to contribute improvements.

---

## 📬 Contact

For questions or suggestions, please reach out via GitHub Issues.

---
