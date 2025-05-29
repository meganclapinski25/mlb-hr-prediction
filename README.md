<h1>⚾️ Predicting Home Runs in MLB Using Swing Metrics</h1> 

<p> This project uses MLB Stacast data from Baseball Savent to build a logistic regression model that predicts whether a plyer will hit at least one homerun based on their swing metrics</p>

<h2> Project Objective</h2>
<p>To explore whether swing metrics such as bat speed, barrel rate, and launch angle can predict if a player is likely to hit a home run. This is accomplished by:</p>
<li>Analyzing swing-related features</li>
<li> Training a logistic regression model</li>
<li>Evaluating model performance</li>

<h2>Features Used</h2>

Key swing metrics included:
- `launch_speed`
- `launch_angle`
- `bat_speed`
- `barrels_total`
- `barrels_per_pa_percent`
- `hardhit_percent`
- `iso` (Isolated Power)
- `bbdist` (Batted Ball Distance)

<h2> Workflow</h2>

1. **Data Cleaning**
   - Created a binary target variable `is_hr` (1 = hit at least one HR, 0 = did not)
   - Handled missing values
   - Selected swing-specific metrics for analysis

2. **Exploratory Data Analysis (EDA)**
   - Visualized distribution of `is_hr`
   - Analyzed boxplots and scatterplots of swing metrics
   - Used correlation heatmaps to identify relationships
   - Detected outliers in launch angle, bat speed, etc.

3. **Modeling**
   - Applied logistic regression to predict `is_hr`
   - Evaluated model using precision, recall, F1-score, and accuracy

4. **Feature Importance**
   - Examined logistic regression coefficients to identify which features had the most predictive power


<h2>Model Performance</h2>

- **Accuracy**: 85%
- **Precision (Class 1 - Hit HR)**: 0.98
- **Recall (Class 1)**: 0.80
- **Top Predictive Features**: `barrels_total`, `iso`, `barrels_per_pa_percent`

<h2> Insights</h2>

- Players with higher barrel rates and ISO are more likely to hit home runs
- `launch_angle` showed wide variation and lower correlation, suggesting it should not be used alone
- Machine learning confirmed that quality of contact (barrels and exit velocity) is more predictive than just swing angle

<h2>Created by Megan Clapinski</h2>
<h4>Senior ACS Student-Athlete at Dominican University of California</h4>
