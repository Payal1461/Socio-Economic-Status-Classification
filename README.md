# Socio-Economic Status Classification of Indian Districts

This project is on classifying Indian districts into
different socio-economic status (SES) categories using census-based data.

The work uses data from Census 2011 and SECC 2011 and applies standard
machine learning models for classification.

---

## Dataset
The dataset contains district-level socio-economic indicators such as:
- Housing type
- Asset ownership
- Income-related variables
- Demographic information

The final dataset includes 613 districts across India.

---

## Approach
1. Data cleaning and preprocessing  
2. Feature standardization  
3. Construction of SES index using PCA  
4. Classification of districts into:
   - Low SES
   - Medium SES
   - High SES  
5. Training machine learning models

---

## Machine Learning Models Used
- Logistic Regression  
- Random Forest  
- Support Vector Machine (SVM)  
- K-Nearest Neighbors  

---

## Evaluation
Models were evaluated using:
- Accuracy
- F1-score

---

## Result
Among the tested models, Logistic Regression, Random Forest, and SVM showed
good performance for SES classification.

---

## Tools Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## Note
This project was done as part of academic learning to understand how machine
learning can be applied to socio-economic data.
