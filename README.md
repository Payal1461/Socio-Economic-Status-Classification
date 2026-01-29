# Socio-Economic Status Classification of Indian Districts

This project explores how machine learning can be used to analyze and classify
Indian districts based on their socio-economic conditions using official
census-based data.

The study combines data from Census of India 2011 and the Socio-Economic and
Caste Census (SECC) 2011 to construct a socio-economic status (SES) index and
classify districts into Low, Medium, and High SES categories.

---

## Motivation
National and state-level indicators such as HDI or MPI often hide large
inequalities that exist within districts. This project focuses on district-level
analysis to better understand variations in housing conditions, income levels,
and asset ownership across India.

---

## Dataset
Two major government datasets were used:

- **SECC 2011**: housing quality, household deprivation, income groups, and asset ownership  
- **Census 2011 (A-1 tables)**: population and household-level demographic indicators  

After preprocessing and merging, the final dataset consists of **613 Indian districts**.

---

## Methodology

### 1. Data Preparation
- Cleaning and filtering district-level records
- Feature engineering and percentage-based indicators
- Removal of low-variance and highly correlated features
- Standardization of all variables

### 2. SES Index Construction
- Principal Component Analysis (PCA) applied to socio-economic indicators
- First principal component used as a composite SES index
- Districts divided into three categories:
  - Low SES
  - Medium SES
  - High SES

### 3. Machine Learning Models
Supervised classification models trained on the labeled dataset:

- Logistic Regression  
- Random Forest  
- Support Vector Machine (SVM)  
- K-Nearest Neighbors (KNN)  

---

## Evaluation
Model performance was evaluated using:
- Accuracy
- Weighted F1-score
- Confusion matrix analysis

---

## Results
Logistic Regression, Random Forest, and SVM achieved the best performance,
with classification accuracy close to **96–97%**.

The SES categorization produced a nearly balanced distribution across districts:
- Low SES: ~33%
- Medium SES: ~33%
- High SES: ~33%

---

## Key Observations
- Housing quality (pucca vs kuccha houses) strongly influences SES
- Asset ownership such as motor vehicles and refrigerators increases SES scores
- Income groups show a clear separation between Low and High SES districts
- Medium SES districts show limited variation, indicating a development plateau

---

## Limitations
- The analysis relies on Census 2011 and SECC 2011 data, which may not represent current socio-economic conditions.
- District-level aggregation can hide household-level variations.
- PCA captures dominant patterns but may overlook smaller regional or cultural influences.
- The project focuses on classification and analysis rather than real-world deployment.


---

## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib
- Google Colab

---

## Note
This project was carried out as part of academic research to understand how
machine learning techniques can be applied to large-scale socio-economic data.
The primary objective was learning, analysis, and interpretation.
