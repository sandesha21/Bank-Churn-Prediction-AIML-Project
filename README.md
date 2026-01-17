# Bank Churn Prediction

![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15.0-orange.svg)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.2.2-green.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-complete-brightgreen.svg)

## Overview  
This project focuses on predicting customer churn for a retail bank using machine learning. By analyzing customer demographics, financial behavior, and engagement patterns, the model helps the bank identify customers at high risk of leaving and implement targeted retention strategies.

## Objective  
The main objective was to build and optimize predictive models that classify customers as likely to churn or stay. Early identification of churn-prone customers enables the bank to proactively engage them with personalized offers and improve overall customer loyalty.

## Dataset  
- **Source:** Provided as part of the project coursework  
- **Size:** ~10,000+ customer records  
- **Key Features:**  
  - Demographics (age, gender, geography)  
  - Account details (balance, products, credit score)  
  - Engagement metrics (tenure, activity patterns)  
- **Target:** Churn Status (`1` = Churned, `0` = Retained)

## Workflow  
1. **Data Preprocessing** – Cleaned and prepared data by encoding categorical variables, handling imbalances, and scaling features.  
2. **Exploratory Data Analysis (EDA)** – Explored churn patterns and feature correlations using visual and statistical methods.  
3. **Model Development** – Built and compared multiple neural network architectures with techniques like dropout, SMOTE, and optimizer tuning.  
4. **Evaluation & Insights** – Selected the best-performing model and extracted business insights from feature importance analysis.

## Model Performance & Results  
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

## Key Insights  
- **SMOTE technique** significantly improved model performance on imbalanced dataset
- **SGD optimizer** provided better generalization compared to Adam optimizer
- Identified key churn drivers: account tenure, balance, and number of products
- Model successfully balances precision and recall for practical business application
- Enabled data-driven decision-making for targeted customer retention strategies

## Installation & Setup  
```bash
# Clone the repository
git clone <repository-url>
cd bank-churn-prediction

# Install required libraries
pip install tensorflow==2.15.0 scikit-learn==1.2.2 seaborn==0.13.1 matplotlib==3.7.1 numpy==1.25.2 pandas==2.0.3 imbalanced-learn==0.10.1

# Launch Jupyter Notebook (recommended: use v2 for enhanced experience)
jupyter notebook INN_Learner_Notebook_Full_code_sbadwaik_final_v2.ipynb
```

## Usage  
1. **Data Loading:** The notebook automatically loads the `Churn.csv` dataset
2. **Data Preprocessing:** Run cells for data cleaning, encoding, and feature scaling
3. **Model Training:** Execute neural network training with different configurations (6 models total)
4. **Evaluation:** View model performance metrics and comparison results
5. **Business Impact:** Analyze financial implications and ROI of the churn prediction model
6. **Predictions:** Use the trained model for churn prediction on new data

**Recommended:** Use `v2.ipynb` for the best experience with enhanced formatting, table of contents, and business impact analysis.

## File Structure  
- `INN_Learner_Notebook_Full_code_sbadwaik_final_v1.ipynb` - Original analysis and model implementation
- `INN_Learner_Notebook_Full_code_sbadwaik_final_v2.ipynb` - **Enhanced version with improved formatting and business impact analysis**
- `INN_Learner_Notebook_Full_code_sbadwaik_final_v2_backup.ipynb` - Backup of previous v2 version
- `Churn.csv` - Customer dataset with demographics and churn labels
- `README.md` - Project documentation
- `LICENSE` - Project license information

## Tech Stack  
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, TensorFlow/Keras  
- **Tools:** Jupyter Notebook / Google Colab  

## Future Work  
- Implement ensemble methods for improved accuracy
- Deploy model as REST API for real-time predictions
- Add feature importance visualization dashboard
- Explore advanced techniques like XGBoost and Random Forest
- Integrate with customer relationship management (CRM) systems

## Author  
**Sandesh S. Badwaik**  
- [LinkedIn](https://www.linkedin.com/in/sbadwaik/)
