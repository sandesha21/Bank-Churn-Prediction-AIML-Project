# Bank Churn Prediction

![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15.0-orange.svg)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.2.2-green.svg)
![Pandas](https://img.shields.io/badge/pandas-2.0.3-blue.svg)
![NumPy](https://img.shields.io/badge/numpy-1.25.2-blue.svg)
![Matplotlib](https://img.shields.io/badge/matplotlib-3.7.1-blue.svg)
![Seaborn](https://img.shields.io/badge/seaborn-0.13.1-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-complete-brightgreen.svg)
![Accuracy](https://img.shields.io/badge/accuracy-79%25-green.svg)
![Recall](https://img.shields.io/badge/recall-69%25-green.svg)

## 📋 Table of Contents
- [🏷️ Keywords & Topics](#️-keywords--topics)
- [📖 Overview](#-overview)
- [🎯 Objective](#-objective)
- [📊 Dataset](#-dataset)
- [🔄 Workflow](#-workflow)
- [📈 Model Performance & Results](#-model-performance--results)
- [🔍 Key Insights](#-key-insights)
- [🚀 Quick Start](#-quick-start)
- [📊 Usage Guide](#-usage-guide)
- [📁 File Structure](#-file-structure)
- [🛠️ Tech Stack](#️-tech-stack)
- [🚀 Future Work](#-future-work)
- [👨‍💻 Author](#-author)

---

## 🏷️ Keywords & Topics

**Primary Keywords:** Data Science • Machine Learning • Neural Networks • Python • Customer Churn Prediction  
**Technical Stack:** TensorFlow • Keras • Scikit-Learn • Pandas • SMOTE • Data Preprocessing • Model Evaluation  
**Business Focus:** Customer Retention • Churn Analytics • Risk Assessment • Business Intelligence • Financial Impact Analysis  
**Industry:** Banking • Financial Services • Customer Analytics • Predictive Modeling • Business Strategy  

**Project Type:** Neural Network Classification | Industry: Banking & Finance | Focus: Customer Retention & Churn Prevention

---

## 📖 Overview  
This project focuses on predicting customer churn for a retail bank using neural network-based machine learning. By analyzing customer demographics, financial behavior, and engagement patterns, the model helps the bank identify customers at high risk of leaving and implement targeted retention strategies.

*For detailed project requirements and specifications, see [PROJECT_REQUIREMENTS.md](PROJECT_REQUIREMENTS.md)*

## 🎯 Objective  
Build a neural network-based classifier that can determine whether a bank customer will leave or not in the next 6 months.

## 📊 Dataset  
- **Source:** Open-source dataset from Kaggle  
- **Size:** 10,000 customer records  
- **Features:** 14 distinct features including demographics, account details, and engagement metrics
- **Target:** Churn Status (`1` = Churned, `0` = Retained)

*Complete data dictionary available in [PROJECT_REQUIREMENTS.md](PROJECT_REQUIREMENTS.md)*

---

## 🔄 Workflow  
1. **Data Preprocessing** – Cleaned and prepared data by encoding categorical variables, handling imbalances, and scaling features.  
2. **Exploratory Data Analysis (EDA)** – Explored churn patterns and feature correlations using visual and statistical methods.  
3. **Model Development** – Built and compared multiple neural network architectures with techniques like dropout, SMOTE, and optimizer tuning.  
4. **Evaluation & Insights** – Selected the best-performing model and extracted business insights from feature importance analysis.

---

## 📈 Model Performance & Results  
**Best Performing Model:** Neural Network with SMOTE & SGD  
- **Training Accuracy:** 85%  
- **Validation Accuracy:** 79%  
- **Precision:** 0.49 (Class 1 - Churned)  
- **Recall:** 0.69 (Class 1 - Churned)  
- **F1-Score:** 0.57 (Class 1 - Churned)  

**Model Comparison (Recall Scores):**
- NN with SMOTE & Adam: 0.259
- NN with SMOTE & Adam & Dropout: 0.179  
- NN with Adam: 0.140
- NN with SGD: 0.037
- NN with Adam & Dropout: 0.034
- **NN with SMOTE & SGD: 0.026** (Best Generalizer - Lowest Overfitting)

---

## 🔍 Key Insights  
- ✅ **SMOTE technique** significantly improved model performance on imbalanced dataset
- ✅ **SGD optimizer** provided better generalization compared to Adam optimizer
- ✅ Identified key churn drivers: account tenure, balance, and number of products
- ✅ Model successfully balances precision and recall for practical business application
- ✅ Enabled data-driven decision-making for targeted customer retention strategies

---

## 🚀 Quick Start

```bash
# 1. Clone the repository
git clone <repository-url>
cd bank-churn-prediction

# 2. Install dependencies
pip install -r requirements.txt
# OR install manually:
pip install tensorflow==2.15.0 scikit-learn==1.2.2 seaborn==0.13.1 matplotlib==3.7.1 numpy==1.25.2 pandas==2.0.3 imbalanced-learn==0.10.1

# 3. Launch Jupyter Notebook
jupyter notebook Bank_Churn_Prediction_Neural_Network_v2.ipynb
```

> 💡 **Tip:** Use `v2.ipynb` for the best experience with enhanced formatting, table of contents, and business impact analysis.

---

## 📊 Usage Guide
1. **📁 Data Loading:** The notebook automatically loads the `Churn.csv` dataset
2. **🔧 Data Preprocessing:** Run cells for data cleaning, encoding, and feature scaling
3. **🤖 Model Training:** Execute neural network training with different configurations (6 models total)
4. **📈 Evaluation:** View model performance metrics and comparison results
5. **💰 Business Impact:** Analyze financial implications and ROI of the churn prediction model
6. **🔮 Predictions:** Use the trained model for churn prediction on new data

---

## 📁 File Structure  
```
├── Bank_Churn_Prediction_Neural_Network_v1.ipynb       # Original analysis and model implementation
├── Bank_Churn_Prediction_Neural_Network_v2.ipynb       # Enhanced version with improved formatting & business impact
├── Churn.csv                                           # Customer dataset (10k records, 14 features)
├── PROJECT_REQUIREMENTS.md                             # Detailed business context & data dictionary
├── README.md                                           # This file
└── LICENSE                                             # Project license information
```

---

## 🛠️ Tech Stack  
- **Language:** Python 3.8+
- **ML Frameworks:** TensorFlow/Keras, Scikit-learn
- **Data Processing:** Pandas, NumPy, Imbalanced-learn (SMOTE)
- **Visualization:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook / Google Colab

---

## 🚀 Future Work  
- 🔄 Implement ensemble methods for improved accuracy
- 🌐 Deploy model as REST API for real-time predictions
- 📊 Add feature importance visualization dashboard
- 🌳 Explore advanced techniques like XGBoost and Random Forest
- 🔗 Integrate with customer relationship management (CRM) systems

---

## 👨‍💻 Author  
**Sandesh S. Badwaik**  
*Data Scientist & Machine Learning Engineer*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sbadwaik/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sandesha21)


---

### 🌟 If you found this project helpful, please give it a ⭐!