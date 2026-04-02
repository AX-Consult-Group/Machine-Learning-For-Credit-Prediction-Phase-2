# Machine-Learning-For-Credit-Prediction-Phase-2

### Background and Aim 

In the first phase of this project, we demonstrated the value of psychometric data as an alternative input for credit scoring, particularly in thin-file markets where traditional financial histories are limited. Using the same 13 higher-order factors, we evaluated five modelling approaches to determine which most effectively ranks credit risk.

Our findings showed that while traditional logistic regression provides a stable and interpretable baseline, more advanced ensemble methods offer improved predictive performance by capturing non-linear relationships and complex interactions between variables. These results highlight the potential for modern machine learning techniques to enhance credit risk assessment and improve applicant selection.

Conventional credit risk underwriting typically relies on linear models such as logistic and conditional logistic regression. These approaches are widely used due to their transparency and ease of interpretation, allowing financial institutions to clearly link individual predictors to outcomes. However, this simplicity may limit their ability to capture more complex behavioral patterns underlying credit risk. 

Building on Phase 1, the aim of this analysis is to explore how different modelling approaches — ranging from traditional linear models to more dynamic machine learning techniques — capture variation in credit risk. In particular, the analysis seeks to assess whether advanced models can uncover hidden structures or interactions that improve the classification of credit outcomes.

### Methods

To address this, we implement and compare a range of modelling techniques with increasing flexibility and complexity: 

1. Conditional Logistic Regression: A traditional, interpretable baseline model commonly used in credit risk modelling.

2. Neural Network Model using Keras/TensorFlow package: A non-linear model capable of capturing complex interactions between predictors.

3. Clustering Techniques - Hierarchical Clustering & K-Means Clustering: Unsupervised approaches used to identify latent subgroups within the data that may exhibit different risk patterns. 

4. XGBoost with Logistic Calibration Layer: A powerful ensemble method that models non-linearities and interactions, with an additional calibration step to produce interpretable probability estimates.

### Data

This analysis uses real **psychometric assessment data**. The scores have been scaled such that risk reduces as the score increases. Additionally, the scores were mapped to a range of 0 to 100.

To protect intellectual property, the names of the DRA variables have been generalized or renamed in this public version. The underlying constructs and relationships remain representative of the actual assessment.

**All financial data** (accounts, arrears, age on book, bad outcome) is simulated to match realistic distributions, correlations, and patterns from the original analysis (based on a South African thin-file population). No real candidate or client information is included.
