# Credit_Card_Fraud_Detection

**Dataset Overview**

The dataset contains 30 features, including time, transaction amount, and anonymized principal components derived from PCA. The target variable, Class, indicates whether a transaction is fraudulent (1) or legitimate (0).

**Key Features:**

Time – Time elapsed since the first transaction

Amount – Transaction amount

V1 - V28 – Anonymized features from PCA transformation

Class – Target variable (0 = Legitimate, 1 = Fraudulent)

**Importing Libraries and Dataset**

To begin, we import essential libraries:

NumPy – For numerical computations

Pandas – For data handling and manipulation

Matplotlib & Seaborn – For visualization

Scikit-Learn – For machine learning and model evaluation

The dataset is loaded using pandas.read_csv() and initial exploration is conducted using head(), shape(), and describe() functions.

**Data Preprocessing and Visualization**

Checked for missing values and handled any inconsistencies.

Identified fraud cases to observe class imbalance, revealing that fraudulent transactions are significantly fewer than legitimate ones.

Visualized distribution of transaction amounts and detected fraudulent transaction patterns using histograms and boxplots.

Generated a heatmap to understand feature correlations, highlighting the relationships between different PCA components and fraud occurrences.

**Splitting Dataset**

Separated the dataset into features (X) and target variable (y).

Used train_test_split() to split data into training (80%) and testing (20%) sets.

**Model Training and Evaluation**

Since fraud detection is a classification problem, we used the following models:

Logistic Regression – A simple baseline model.

K-Nearest Neighbors (KNN) – Used for pattern recognition in transactions.

Random Forest Classifier – Employed for feature importance analysis.

Support Vector Classifier (SVC) – Used for separating fraudulent and legitimate transactions.

**Conclusion**

The Random Forest Classifier achieved the highest accuracy of 98%, effectively detecting fraudulent transactions. Hyperparameter tuning and feature selection further improved the model’s precision and recall, reducing false positives while maintaining a high detection rate.
