# Loan Approval Prediction System

## Introduction:
This project aims to predict loan approval status using customer and asset data. By applying data science techniques, we analyze key factors influencing loan decisions and build a logistic regression model from scratch. The workflow includes data exploration, preprocessing, visualization, and model evaluation.

---


## Data Description:
The dataset (`loan_approval_dataset.csv`) contains the following columns:
- **no_of_dependents**: Number of dependents
- **education**: Education status (Graduate/Not Graduate)
- **self_employed**: Employment status (Yes/No)
- **income_annum**: Annual income
- **loan_amount**: Requested loan amount
- **loan_term**: Loan term (months)
- **cibil_score**: CIBIL credit score
- **residential_assets_value**: Value of residential assets
- **commercial_assets_value**: Value of commercial assets
- **luxury_assets_value**: Value of luxury assets
- **bank_asset_value**: Value of bank assets
- **loan_status**: Target variable (Approved/Rejected)

---


## Preprocessing:
- **Missing Values**: Checked and handled missing values.
- **Label Encoding**: Converted categorical columns (`education`, `self_employed`, `loan_status`) to numerical values using `LabelEncoder`.
- **Feature Selection**: Selected relevant features for modeling.
- **Scaling**: Standardized numerical features using `StandardScaler`.

---


## Exploratory Data Analysis (EDA):

### 1. Data Overview
- Checked shape, columns, info, and summary statistics.

### 2. Target Variable Distribution
- Visualized the distribution of approved vs rejected loans.
![Distribution of Loan Status](plotsImages/target_distribution.png)

### 3. Categorical Feature Analysis
- Explored how education and employment status affect loan approval.
![Education vs Loan Status](plotsImages/Categorical_Features/categorical_feature1.png)
![Self-employed vs Loan Status](plotsImages/Categorical_Features/categorical_feature2.png)

### 4. Numerical Feature Distributions
- Plotted histograms for all numerical features.
![Numerical Features](plotsImages/numerical_feature_histogram.png)

### 5. Boxplots: Numerical Features vs Target
- Compared distributions of numerical features for approved vs rejected loans.
![Numerical Features vs Target](plotsImages/numerical_vs_target.png)

### 6. Correlation Analysis
- Visualized feature correlations.
![Correlation Analysis](plotsImages/correlation_matrix.png)

### 7. Scatter Plots: Feature vs Target
- Plotted each feature against the target variable.
![All Features vs Target](plotsImages/features_vs_target.png)

### 8. Pairplot for Feature Interactions
- Explored pairwise relationships between features.
![Features Pairplot](plotsImages/pairplots_features.png)

---


## Model:
- Implemented logistic regression from scratch using gradient descent.
- Functions: `sigmoid`, `cost`, `gradient`, `GradientDescent`, `Prediction`.

---


## Model EDA & Plots:
### 1. Cost Function Visualization
- Shows model learning progress.
![Cost function for learing process](plotsImages/cost_function.png)

### 2. Prediction Distribution
- Visualizes predicted loan status.
![Prediction distribution for approved and rejected persons](plotsImages/prediction_distribution.png)

### 3. Model Accuracy
- Shows the proportion of correct vs incorrect predictions.
![Model Accuracy (in %)](plotsImages/accuracy.png)

### 4. Confusion Matrix (Optional)
- Evaluates model accuracy.
![Confusion matrix](plotsImages/confusion_matrix.png)
---


## Conclusion:
This project demonstrates a full machine learning workflow for loan approval prediction, including data cleaning, EDA, feature engineering, custom model implementation, and result visualization. The approach provides insights into the factors affecting loan approval and a baseline model