
# ⚾️ Predicting Home Runs in MLB Using Swing Metrics

 Using MLB Stacast data from Baseball Savent to build a logistic regression model that predicts whether a plyer will hit at least one homerun based on their swing metrics




## Authors

- [@meganclapinski](https://www.github.com/meganclapinski25)


## Features

- Logistic Regression Classifier
- Real Statcast data analysis
- EDA visualizations of home run distributions
- Feature importance analysis
- Outlier detection 


## Workflow

-  Clean and preprocess the dataset
-  Create a binary target variable (`is_hr`)
- Analyze swing-related metrics via EDA
- Train logistic regression model
- Evaluate model with precision, recall, F1-score
- Visualize top predictors and outliers
## Results

- Model Accuracy: 85%
- Key Predictors: `barrels_total`, `iso`, `barrels_per_pa_percent`
- Players with better barrel quality were more likely to hit HRs


## Visual Highlights

### 🎯 Model Performance: Confusion Matrix
![Confusion Matrix] (images/confusion.png)

### 📈 Key Swing Metrics Correlated with Home Runs
![Feature Correlation] (images/correlation.png)

### 🔍 Model Interpretation: Feature Weights
![Feature Weights] (images/weights.png)