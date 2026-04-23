#  Supplier Risk Classifier

An end-to-end Machine Learning project designed to evaluate and predict supplier risk in supply chains. By analyzing historical supplier data, this model classifies suppliers as **'Safe'** or **'At-Risk'**, helping businesses proactively mitigate supply chain disruptions.

##  Project Overview
Supply chain failures can cost businesses millions. This project builds a predictive model to identify at-risk suppliers before they fail. The model analyzes 1,000 suppliers using business-critical metrics to determine the probability of failure.

**Key Highlights:**
- **Business-Centric Tuning:** The model's decision threshold is explicitly tuned to prioritize recall (catching risky suppliers), ensuring a business threshold of ~0.94.
- **Handling Imbalance:** Utilized **SMOTE** to handle class imbalances between Safe and At-Risk suppliers.
- **Algorithm Comparison:** Evaluated Logistic Regression, Support Vector Machines (SVM), and Linear Discriminant Analysis (LDA).
- **Automated Reporting:** Generates a Batch Risk Scoring Report to rank suppliers by risk probability.

##  Top Risk Drivers Identified
By interpreting the model's weights, the top 5 factors driving supplier risk were identified as:
1. **Defect Trajectory**
2. **Recent 3-Month Defect Rate**
3. **Debt Ratio**
4. **Lifetime Defect Rate**
5. **Financial Health Score**

## 📈 Model Performance
**Logistic Regression** outperformed the others in business utility, achieving:
* **ROC-AUC Score:** ~0.986
* **Average Precision:** ~0.915
* Lowest number of missed risks (False Negatives)

##  Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn, Imbalanced-Learn (SMOTE)
* **Visualization:** Matplotlib, Seaborn

## 🚀 How to View the Code
Simply open the `Supplier_risk_classifier_ML_project.ipynb` file in this repository to view the full data pipeline, visualizations, cross-validation, and final risk reporting.
