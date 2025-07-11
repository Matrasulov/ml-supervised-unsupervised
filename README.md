# Supervised and Unsupervised Machine Learning Projects

This repository contains a set of supervised and unsupervised machine learning projects built using regression, classification, and clustering techniques on real-world datasets: `exams.csv` and `college.csv` for supervised tasks, and `humanitarian.csv` and `customer.csv` for unsupervised clustering.

---

## 1. Supervised Learning

### Objective
To build regression and classification models using the `exams.csv` and `college.csv` datasets and evaluate their performance.

### Workflow

#### a. Understanding Regression vs Classification
A brief comparative report is included that highlights the key differences between regression and classification tasks, supported with examples.

#### b. Dataset Preparation
- Downloaded datasets using a custom data-fetching function.
- Performed exploratory data analysis (EDA).
- Visualized distributions, relationships, and feature correlations.

#### c. Exploratory Data Analysis – `exams.csv`
Includes key visual insights:
- Gender distribution (Pie Chart)  
  <img width="636" height="660" alt="gender" src="https://github.com/user-attachments/assets/a0169da0-bc01-4285-8d84-5e6fadd59b5e" />


- Race/Ethnicity distribution (Bar Chart)  
  <img width="1990" height="989" alt="image" src="https://github.com/user-attachments/assets/10fa0da8-59de-449b-bd87-cc03d0142dc6" />


- Parental level of education (Bar Chart)  
  <img width="1990" height="990" alt="image" src="https://github.com/user-attachments/assets/49e244cd-bd5f-4c65-891c-f0d1a35bad5f" />


#### d. Feature Engineering
- **Target (y)**: `math score`
- **Features (X)**: `reading score`, `writing score`, `gender`, `race`, `parental level of education`, `lunch`, `test preparation course`

#### e. Preprocessing
- Standardized numerical features using `StandardScaler`
- Encoded categorical variables using `OneHotEncoder`

#### f. Model Training and Evaluation

- Trained and evaluated:
  - `LinearRegression`
  - `DecisionTreeRegressor`
  - `RandomForestRegressor`

- **Model Comparison (R² Score Bar Chart)**  
  <img width="691" height="470" alt="image" src="https://github.com/user-attachments/assets/bb6aa5ba-a459-4edb-bb27-8ef103c5163d" />


#### g. Experiments on Alternate Targets – `exams.csv`
- Additional regression tasks:
  - Target: `writing score`
  - Target: `reading score`
- Excluded new target from feature set in each case

---

## 2. Unsupervised Learning

### Objective
To explore clustering techniques using `college.csv`, `humanitarian.csv`, and `customer.csv`.

### Workflow

#### a. Exploratory Data Analysis – `humanitarian.csv`
- Correlation Heatmap  
  <img width="836" height="528" alt="image" src="https://github.com/user-attachments/assets/ad654601-1009-4b1f-b532-157f8ed3f693" />


#### b. Elbow Method (Income vs GDP, etc.)
- Applied Elbow Method on selected feature pairs to determine optimal clusters  
  <img width="536" height="393" alt="image" src="https://github.com/user-attachments/assets/f9eec43c-31bb-49ae-8f75-3a735065c18b" />


#### c. Clustering – KMeans
- Performed KMeans clustering on selected feature combinations
- **Scatter Plot of Cluster Assignments**  
<img width="566" height="470" alt="image" src="https://github.com/user-attachments/assets/17e068d8-4184-4cee-a491-450c0a1addef" />
<img width="532" height="470" alt="image" src="https://github.com/user-attachments/assets/dd278899-4f44-44cc-8956-d6b98b32c1f8" />
<img width="523" height="470" alt="image" src="https://github.com/user-attachments/assets/0f3b4dc3-5b0f-443f-a2de-fb56d7266f4a" />
<img width="540" height="470" alt="image" src="https://github.com/user-attachments/assets/8c4866ce-1764-4480-a051-7df4561f80cf" />



---

## Tools & Libraries
- Python (Jupyter Notebook)
- Scikit-learn
- Pandas, NumPy
- Matplotlib, Seaborn

---

## Author
**Akbarjon Matrasulov**  
AI & Data Science Student
