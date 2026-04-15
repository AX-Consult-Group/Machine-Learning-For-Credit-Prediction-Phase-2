# machine-learning-for-credit-prediction-phase-2

### Background and Aim 

In the first phase of this project, we demonstrated the value of psychometric data as an alternative input for credit scoring, particularly in thin-file markets where traditional financial histories are limited. Using the same 13 higher-order factors, we evaluated five modelling approaches to determine which most effectively ranks credit risk.

Traditional credit scoring models have served as the foundation for consumer risk assessment for decades. Logistic regression, in particular, remains widely used due to its transparency and interpretability, allowing financial institutions and regulators to clearly link individual predictors to outcomes. However, these conventional approaches have important limitations. For example, they typically assume linearity and independence among predictors, which restricts their ability to capture complex interactions and non-linear behavioral patterns. 

Building on Phase 1, the aim of this analysis is to explore how different modelling approaches — ranging from traditional linear models to more advanced Machine Learning (ML) techniques — capture variation in credit risk. In particular, we seek to assess whether modern ML methods can uncover hidden structures, complex interactions, and behavioral signals that improve the classification of credit outcomes beyond what is possible with conventional approaches.

Our findings from Phase 1 showed that while traditional logistic regression provides a stable and interpretable baseline, ensemble methods such as XGBoost offer improved predictive performance by better capturing non-linear relationships. This phase extends that work by incorporating psychometric DRA scores into a broader range of techniques, including neural networks and clustering, to evaluate their ability to enhance risk assessment. 

--- 

### Methods

To address this, we implement and compare a range of modelling techniques with increasing flexibility and complexity: 

1. Conditional Logistic Regression: A traditional, interpretable baseline model commonly used in credit risk modelling.

2. Neural Network using Keras/TensorFlow package: A non-linear model capable of capturing complex interactions between predictors.

3. Clustering Techniques - Hierarchical Clustering & K-Means Clustering: Unsupervised approaches used to identify latent subgroups within the data that may exhibit different risk patterns. 

4. XGBoost: A gradient boosting ensemble model that captures non-linear interactions among variables.

5. Hybrid Model (XGBoost + Logistic Calibration + Scorecard): XGBoost predictions were passed through a logistic calibration layer to produce well-calibrated probabilities, which were then transformed into an interpretable scorecard with risk bands A–F.

---

### Data

This analysis uses real **psychometric assessment data**. The scores have been scaled such that risk reduces as the score increases. Additionally, the scores were mapped to a range of 0 to 100.

To protect intellectual property, the names of the DRA variables have been generalized or renamed in this public version. The underlying constructs and relationships remain representative of the actual assessment.

**All financial data** (accounts, arrears, age on book, bad outcome) is simulated to match realistic distributions, correlations, and patterns from the original analysis (based on a South African thin-file population). No real candidate or client information is included.

---

## How to view the report

The full rendered report is available via **GitHub Pages**: 

xxx

---

### Technologies used
The analysis was conducted in R using the following packages:

### Analysis
- xgboost
- shapviz
- MatchIt
- lm.beta
- reticulate
- keras3
- tensorflow
- cluster
- factoextra

---

R Version 4.5.3
R Studio Version 2026.01.1+403
