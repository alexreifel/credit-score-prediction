# Credit Score Prediction

This project explores multiclass credit-score classification using demographic and financial-behavior variables.

The goal is to predict whether an individual's credit score falls into the **Poor**, **Standard**, or **Good** category while examining which financial characteristics are most useful for distinguishing between the three groups.

## Workflow

The analysis includes:

- Cleaning inconsistent numerical and categorical values
- Handling missing data
- Converting credit-history age into a numerical feature
- Encoding categorical variables
- Engineering indicators for loan types and payment behavior
- Scaling numerical features for predictive analysis
- Exploratory analysis and visualization
- Training and evaluating an XGBoost classifier

## Model Results

The final XGBoost model was trained on 80,000 observations and evaluated on a 20,000-observation test set.

**Overall test accuracy: 69.56%**

Class-level performance:

- **Poor:** precision 0.68, recall 0.77, F1 0.72
- **Standard:** precision 0.84, recall 0.61, F1 0.71
- **Good:** precision 0.52, recall 0.82, F1 0.63

The results show that overall accuracy alone hides meaningful class-level tradeoffs. The model identifies a large share of Good-credit observations but with lower precision, while Standard-credit predictions are more precise but miss a larger share of true cases.

## Notebook

The Jupyter notebook contains the complete data-cleaning, feature-engineering, exploratory-analysis, modeling, and evaluation workflow.

[View Notebook](Predicting%20Credit%20Scores%20Using%20Demographic%20and%20Financial%20Data.ipynb)

## Tools

Python · pandas · NumPy · scikit-learn · XGBoost · category encoders · Matplotlib · seaborn · Jupyter
