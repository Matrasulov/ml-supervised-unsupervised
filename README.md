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
- Downloaded `exams.csv` and `college.csv` using a custom data-fetching function.
- Performed exploratory data analysis (EDA).
- Visualized distributions, relationships, and feature correlations.

#### c. Exploratory Data Analysis – `exams.csv`
Includes key visual insights:
- Gender distribution (Pie Chart)  
  ![Gender Pie Chart](images/gender_pie_chart.png)

- Race/Ethnicity distribution (Bar Chart)  
  ![Race/Ethnicity Bar Chart](images/race_ethnicity_bar.png)

- Parental level of education (Bar Chart)  
  ![Parental Education Bar Chart](images/parental_education_bar.png)

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
  ![Model Comparison](images/model_comparison_r2.png)

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

#### a. Exploratory Data Analysis – `college.csv`
- Correlation Heatmap  
  ![Correlation Heatmap](images/college_correlation_heatmap.png)

#### b. Elbow Method (Income vs GDP, etc.)
- Applied Elbow Method on selected feature pairs to determine optimal clusters  
  ![Elbow Method](images/elbow_method_income_gdp.png)

#### c. Clustering – KMeans
- Performed KMeans clustering on selected feature combinations
- **Scatter Plot of Cluster Assignments**  
  ![KMeans Clusters](images/kmeans_clusters.png)

#### d. Post-Clustering Supervised Learning
- Added cluster labels as a new `label` column to the dataset
- Trained classification models using newly labeled data

---

## Tools & Libraries
- Python (Jupyter Notebook)
- Scikit-learn
- Pandas, NumPy
- Matplotlib, Seaborn

---

## Author
**Akbarjon Matrasulov**  
Senior-year AI & Data Science Student
