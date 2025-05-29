# Elevatelabs_2

**1. Data Loading & Inspection**

* The dataset is loaded from `Housing.csv` into a pandas DataFrame.
* Initial inspection includes displaying the first few rows and checking the DataFrame’s shape.
* Error handling is implemented for file-related issues.

**2. Exploratory Data Analysis (EDA)**

* Data types and descriptive statistics are examined.
* Missing values are identified.
* Key visualizations include:

  * Histograms (price, area), boxplot (price), scatter plot (price vs area).
  * Bar plots for categorical feature distributions.
  * Correlation heatmap for numerical features.

**3. Data Preprocessing**

* Outliers in 'price' and 'area' capped at the 95th percentile.
* Categorical variables encoded via one-hot encoding.
* Numerical features (excluding 'price') scaled using `StandardScaler`.

**4. Data Splitting**

* Features (`X`) and target (`y = price`) are defined.
* Data is split into training (80%) and test (20%) sets.

**5. Model Training**

* Two linear regression models developed:

  * Simple Linear Regression using 'area' as the sole predictor.
  * Multiple Linear Regression using all preprocessed features.

**6. Model Evaluation**

* Predictions made on the test set.
* Evaluation metrics: MAE, MSE, and R² score.

**7. Visualization of Results**

* Scatter plot for actual vs. predicted values (simple regression).
* Bar plot of feature coefficients (multiple regression).
* Scatter plots for top influential features with regression lines.

**8. Model Refinement & Regularization**

* Insignificant features (based on coefficients) removed.
* Model retrained and re-evaluated.
* Ridge and Lasso regularization applied with varying alpha values, and performance metrics compared.
