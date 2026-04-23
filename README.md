# **Data Preprocessing & Exploratory Data Analysis (EDA)**  
## Course Information  
- University: Birzeit University
- Faculty: Engineering and Technology
- Department: Computer Engineering
- Course: ENCS5341 – Machine Learning and Data Science
- Assignment: #1 – Data Preprocessing & EDA

## Project Overview  
This project focuses on the first phase of the data science pipeline, including:
- Data Cleaning
- Handling Missing Values
- Outlier Detection & Treatment
- Feature Scaling
- Exploratory Data Analysis (EDA)

The dataset simulates real-world customer behavior to analyze factors affecting customer churn.

## Objectives  
- Prepare raw data for machine learning
- Understand feature distributions
- Discover relationships between variables
- Identify key predictors of churn

## Dataset  
- Records: 3,500
- Features: 8
- Target Variable: ChurnStatus
- Features:
  - Age
  - Income
  - Tenure
  - SupportCalls
  - Gender
  - ProductType
## Workflow  
1. Data Inspection
   - Used .head(), .info(), .describe()
   - Identified missing values in multiple columns
     
2️. Missing Values Handling
   - Numerical: Median Imputation
   - Categorical: Mode Imputation
   Result: Clean dataset with no missing values

3️. Outlier Handling
  - Method: IQR (Interquartile Range)
  - Technique: Median Replacement
Preserves data distribution while removing extreme effects

4️. Feature Scaling
  - Method: Z-score Standardization
    Ensures all features are on the same scale
    Improves model performance

5️. Exploratory Data Analysis (EDA)
- Univariate Analysis
  - Histograms (numerical features)
  - Bar plots (categorical features)
- Bivariate Analysis
  - Boxplots (feature vs churn)
  - Bar plots (categorical relationships)
- Correlation Analysis
  - Heatmap of feature relationships
  - Focus on correlation with churn
    
## Key Insights
- Most Predictive Features
  - Tenure → Strong negative correlation
  - Income → Moderate negative correlation
  - SupportCalls → Weak positive correlation
  - Age → No significant impact
## Behavioral Patterns
- Low tenure → High churn
-  Lower income → Higher churn
-   More support calls → Potential dissatisfaction
-   Gender & ProductType → Minimal influence

## Visualizations
- Correlation Heatmap
- Histograms & Distributions
- Boxplots (Churn vs Features)
- Scatter Plot (Tenure vs Income)
- Bar Charts (Categorical Analysis)

## Conclusion
- Data preprocessing significantly improved dataset quality
- Tenure is the strongest churn indicator
- Early-stage customers require more retention efforts
- Clean, scaled data is ready for ML modeling

## Repository Structure
```
├── data/              # Dataset files
├── notebook.ipynb    # Main analysis notebook
├── figures/          # Visualizations
├── report.pdf        # Assignment report
└── README.md
```
## Future Work
- Build predictive models (Logistic Regression, Random Forest, etc.)
- Feature engineering
- Hyperparameter tuning
