# 🍽️ Zomato Restaurant Rating Analysis & Machine Learning

An end-to-end Data Analysis and Machine Learning project exploring restaurant ratings, customer preferences, pricing patterns, and restaurant characteristics using the Zomato dataset.

The project combines data cleaning, exploratory data analysis (EDA), feature engineering, and multiple machine learning algorithms to investigate restaurant ratings in Bangalore, India.

## 📌 Project Overview

Restaurant ratings can provide valuable insights into customer satisfaction, restaurant popularity, pricing, and service preferences.

This project analyzes restaurant data to uncover meaningful patterns and builds machine learning models for two tasks:

- **Regression:** Predicting numerical restaurant ratings.
- **Classification:** Categorizing restaurants into high- and low-rating groups.

## 🎯 Objectives

- Clean and preprocess real-world restaurant data.
- Explore rating distributions and restaurant characteristics.
- Identify relationships between pricing, popularity, location, and ratings.
- Engineer useful features from existing columns.
- Prepare categorical and numerical features for machine learning.
- Train and evaluate multiple regression and classification models.
- Compare model performance using appropriate evaluation metrics.

## 📂 Dataset

The project uses the Zomato restaurant dataset containing information about restaurants in Bangalore, India.

Key features include:

| Feature | Description |
|---|---|
| `name` | Restaurant name |
| `online_order` | Whether online ordering is available |
| `book_table` | Whether table booking is available |
| `rate` | Restaurant rating out of 5 |
| `votes` | Number of customer votes |
| `location` | Restaurant neighborhood |
| `rest_type` | Type of restaurant |
| `cuisines` | Cuisines offered |
| `approx_cost(for two people)` | Approximate cost for two people |
| `listed_in(type)` | Restaurant service category |

**Dataset setup:** Place the dataset file named `zomato.csv` in the same directory as the Jupyter Notebook before running the project.

## 🛠️ Technologies & Libraries

- **Python** — Core programming language
- **Pandas & NumPy** — Data manipulation and numerical operations
- **Matplotlib & Seaborn** — Data visualization
- **Scikit-learn** — Preprocessing, model training, and evaluation
- **Jupyter Notebook** — Interactive analysis and experimentation

## 🔍 Project Workflow

### 1. Data Loading & Initial Inspection
- Load the dataset and inspect its structure.
- Examine data types, dataset dimensions, and sample records.
- Identify missing values and potential data quality issues.

### 2. Data Cleaning & Preprocessing
- Convert restaurant ratings into numerical values.
- Handle missing values and remove unsuitable columns.
- Transform binary categorical features into numerical representations.
- Inspect duplicates and data distributions.
- Prepare the dataset for exploratory analysis and modeling.

### 3. Exploratory Data Analysis (EDA)
Investigate several business questions:

- How are restaurant ratings distributed?
- Do online ordering and table booking relate to restaurant ratings?
- How does the approximate cost for two people relate to ratings?
- Which neighborhoods have the highest restaurant concentration?
- Is restaurant popularity, measured by votes, associated with higher ratings?
- Which restaurant types are most common?

### 4. Feature Engineering
Create and transform features to improve model readiness:

- `is_chain` — Indicates whether a restaurant name appears multiple times.
- `has_phone` — Indicates whether a phone number is available.
- `num_cuisines` — Represents the number of cuisines offered.
- Group infrequent categories into an `Others` category.
- Apply One-Hot Encoding to categorical variables.
- Apply log transformations to highly skewed numerical features.

### 5. Regression Models
Train and compare models for predicting numerical restaurant ratings:

- Linear Regression
- K-Nearest Neighbors (KNN) Regressor
- Decision Tree Regressor
- Random Forest Regressor
- AdaBoost Regressor
- Gradient Boosting Regressor

Evaluate model performance using regression metrics and 5-fold cross-validation.

### 6. Classification Models
Convert numerical ratings into two categories using a threshold of 3.75:

- High rating: Rating at or above the threshold.
- Low rating: Rating below the threshold.

Train and evaluate:

- Logistic Regression
- K-Nearest Neighbors (KNN) Classifier
- Gaussian Naive Bayes
- Support Vector Classifier (SVC)
- Decision Tree Classifier
- Random Forest Classifier
- AdaBoost Classifier
- Gradient Boosting Classifier

Use classification evaluation metrics and 5-fold Stratified Cross-Validation to assess model performance and consistency.

## 📊 Key Business Insights

The exploratory analysis investigates the following patterns:

- **Rating distribution:** Restaurant ratings are concentrated around the middle-to-high range.
- **Table booking:** Restaurants offering table booking show higher typical ratings in the exploratory analysis.
- **Pricing:** Higher-priced restaurant groups tend to have higher average ratings.
- **Geographic concentration:** BTM, HSR, and Koramangala emerge as important restaurant hubs.
- **Customer engagement:** Vote counts help explore the relationship between popularity and ratings.
- **Restaurant types:** Quick Bites and Casual Dining represent prominent restaurant categories.

These are exploratory observations and do not, by themselves, establish causation.

## 📈 Model Evaluation

The project compares multiple algorithms rather than relying on a single model.

**Regression:** Assess prediction errors and goodness of fit using metrics such as MAE, RMSE, and R² where reported in the notebook.

**Classification:** Assess predictive performance using metrics such as accuracy, precision, recall, F1-score, and ROC-AUC where applicable.

Five-fold cross-validation is used to investigate model stability across different data splits.

## 💡 What I Learned

- Cleaning and preprocessing a real-world dataset.
- Handling missing values and high-cardinality categorical features.
- Extracting useful information through feature engineering.
- Performing exploratory data analysis and communicating business insights.
- Building regression and classification pipelines.
- Comparing machine learning algorithms using evaluation metrics.
- Applying cross-validation to assess model generalization.

## 🚀 How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR-USERNAME/zomato-restaurant-rating-ml.git
   ```

2. Navigate to the project directory:

   ```bash
   cd zomato-restaurant-rating-ml
   ```

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

4. Ensure that `zomato.csv` is in the project directory.

5. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

6. Open `Zomato_Restaurant_Rating_Analysis.ipynb` and run the cells in order.

## 👩‍💻 Author

**Shahd Ayman Kamal**

Computer Science Student | Data Analysis & Machine Learning Enthusiast

Cairo University — Faculty of Computers and Artificial Intelligence

- GitHub: (https://github.com/Ash20240279)

---

*This project was developed for practical learning and experimentation in data analysis and machine learning.*
