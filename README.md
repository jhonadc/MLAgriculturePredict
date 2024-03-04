# Machine Learning for Crop Prediction

## Project Overview
This project applies machine learning to predict crop types based on soil properties. Utilizing a dataset of soil measures, we employ logistic regression to understand the relationships between soil characteristics and crop viability.

## Data Description
The dataset, `soil_measures.csv`, includes various soil properties such as Nitrogen (N), Phosphorus (P), Potassium (K), and pH level. These features serve as predictors for the types of crops that can be grown.

## Methodology

### Data Exploration and Preprocessing
- The dataset is first explored to understand its structure, including a preliminary look at the top rows and summary statistics.
- Data quality is assessed by checking for missing values, which could impact model accuracy.
- The target variable, `crop`, is analyzed to determine the diversity of crop types in the dataset.

### Feature Engineering
- Features are standardized using `StandardScaler` to ensure uniformity and to aid in the convergence of the logistic regression algorithm.
- A correlation matrix is generated to identify potential multicollinearity between features, which could affect model performance.

### Model Training
- Logistic Regression models are trained for each individual feature to measure their predictive power, using F1-score as the evaluation metric.
- A final logistic regression model is trained on selected features considered most important through exploratory analysis.

### Evaluation
- The final model's performance is evaluated using the F1-score, classification report, and confusion matrix to provide a comprehensive understanding of its predictive capabilities.

## Results
- Feature importance is visualized through a bar plot, highlighting the contribution of each feature to the model's predictive ability.
- The confusion matrix illustrates the model's performance across different classes, identifying areas where the model excels or falls short.

## Usage
The provided Jupyter notebook contains all the code for the project. To replicate the results, run each cell sequentially, from data loading to model evaluation.

## Conclusion
The project demonstrates the capability of logistic regression in predicting crop types based on soil properties. Future work could involve experimenting with other classification algorithms, hyperparameter tuning, and cross-validation to potentially improve model performance.
