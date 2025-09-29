# CustomerChurn
  Project status(Active)

# Project objective
  The telecommunications industry faces persistent challenges with high customer attrition, commonly known as churn, with annual rates often exceeding 20%. Given that acquiring a new customer is significantly more costly than retaining an existing one, predicting and preventing voluntary churn is a top business priority for maintaining profitability and market share. The objective of this project is to develop a robust, data-driven solution for customer retention by leveraging the Telco Customer Churn dataset provided by Kaggle(https://www.kaggle.com/datasets/blastchar/telco-customer-churn). This initiative involves a multi-step analytical approach: (1) Exploratory Data Analysis (EDA) to uncover key demographic, service, and account-related factors that correlate strongly with churn, such as contract type and monthly charges; (2) Statistical Churn Analysis to quantify the impact of specific features; and (3) Predictive Modeling using classification algorithms, like Logistic Regression and Random Forest, to accurately forecast which individual customers are most likely to discontinue their service. The ultimate goal is to generate actionable insights and a reliable model that enables the company to target high-risk customers with proactive, personalized retention offers, thereby minimizing revenue loss and optimizing retention spending.

# Methods
  List with methods:
  1. Data Preprocessing and Exploration

    - Data Loading & Inspection: The initial dataset was loaded, and its structure was inspected using descriptive statistics and data type summaries (info(), describe()).
    - Feature Scaling: Numerical features (tenure, MonthlyCharges, TotalCharges) were standardized using the StandardScaler to ensure equal contribution to model training, preventing features with large values from dominating the learning process.

  2. Exploratory and Statistical Analysis

    - Grouping and Aggregation: Churn rates were calculated by grouping the data across various categorical features (e.g., Contract type, Payment Method, Service Type) to quantify the impact of each segment.
    - Correlation Analysis: A correlation matrix was computed to identify strong relationships between independent variables and the target variable (Churn).

    - Visualization:
      - Distribution Plots (Histograms & Boxplots): Used to visualize the spread of numerical features (tenure, MonthlyCharges) and how their distributions differ between churning and non-churning customers.
      - Count Plots: Used to visualize churn proportions across binary and categorical features.

  3. Predictive Modeling and Evaluation

    - Train-Test Splitting: The dataset was partitioned into 80% training data and 20% testing data using stratified sampling to maintain the original class balance of the target variable (Churn) in both subsets.

    - Model Training: Two classification algorithms were trained:
      - Logistic Regression: Served as a simple, interpretable baseline model.
      - Random Forest Classifier: Used as a more powerful ensemble model to capture non-linear relationships and provide higher predictive performance.

    - Model Evaluation: Performance was assessed on the unseen test data using crucial classification metrics relevant to imbalanced data:
      - Accuracy, Precision, Recall, and F1-Score.
      - ROC-AUC Score: Used to evaluate the model's ability to distinguish between the two classes.
      - Confusion Matrices and ROC Curves: Used to visualize model performance and comparison.
      
    - Feature Importance: The coefficients from the Logistic Regression model were used to rank features by their predictive strength for churn, providing key business insights.

# Technologies 
  List with used technologies:
  - Python: The primary programming language used for all data processing and modeling tasks.
  - Pandas: Used extensively for data loading, structuring, filtering, grouping, and aggregation during the EDA phase.
  - NumPy: Used for high-performance numerical operations and array manipulations, foundational to the machine learning algorithms.
  - Matplotlib: The core library used for generating static, publication-quality visualizations, including the ROC curves and confusion matrices.
  - Seaborn: Built on Matplotlib, used for creating visually appealing statistical graphics, such as boxplots, histograms, and heatmaps for the correlation analysis.
  - Scikit-learn (sklearn): The central library for predictive modeling, specifically used for:
    - Preprocessing: StandardScaler for feature scaling.
    - Data Splitting: train_test_split for creating training and testing sets.
    - Model Training: LogisticRegression and RandomForestClassifier.
    - Evaluation: Calculating all performance metrics (accuracy_score, roc_auc_score, confusion_matrix, etc.).

# Project Description
  Paragraph with a description of the dataset, sources, characteristics ,etc.

# Steps
  Add here any insights you had during the project

# Conclusion
  Final conclusion
  
# Contact
  linkedin, github, medium, etc 