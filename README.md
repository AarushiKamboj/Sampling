# Sampling

#Credit Card Fraud Detection and Sampling Techniques
#Overview
Credit card fraud detection is a critical task to ensure the security of financial transactions. This project addresses the initial challenge of imbalanced data, where only 9 out of 772 transactions are labeled as fraudulent. To mitigate this imbalance, oversampling techniques are employed, creating additional instances of the minority class (fraudulent cases) to balance the dataset.

#Dataset
The dataset consists of credit card transactions with 30 features, and the class labels indicate whether a transaction is fraudulent (1) or not (0). Initially, the class distribution is highly imbalanced, with 763 non-fraudulent cases and only 9 fraudulent cases.

#Sampling Techniques
#1. Simple Random Sampling
Technique Description: Random selection of samples from the population.
Results:
Random Forest: 0.9870
Logistic Regression: 0.8831
Naive Bayes: 0.7013
Decision Trees: 0.9610
KNN: 0.8701
#2. Systematic Sampling
Technique Description: Regular interval selection after a random start.
Results:
Random Forest: 1.0000
Logistic Regression: 0.8926
Naive Bayes: 0.7450
Decision Trees: 1.0000
KNN: 0.9329
#3. Cluster Sampling
Technique Description: Randomly selecting clusters from the population.
Results:
Random Forest: 1.0000
Logistic Regression: 0.9670
Naive Bayes: 1.0000
Decision Trees: 1.0000
KNN: 0.9890
#4. Stratified Sampling
Technique Description: Division of the population into subgroups based on certain criteria.
Results:
Random Forest: 1.0000
Logistic Regression: 0.9030
Naive Bayes: 0.7239
Decision Trees: 0.9925
KNN: 0.9552
#5. Bootstrap Sampling
Technique Description: Resampling with replacement to create multiple samples from the original dataset.
Results:
Random Forest: 1.0000
Logistic Regression: 0.9250
Naive Bayes: 0.7500
Decision Trees: 0.9625
KNN: 0.9375
#Conclusion
In summary, each sampling technique was applied to create five distinct samples, and five different machine learning models were trained on each sample. The Random Forest model consistently achieved high accuracy across various sampling techniques. Notably, when applied to the Stratified Sampling technique, the Random Forest model outperformed all other models, yielding perfect accuracy. These findings provide insights into the effectiveness of different sampling techniques in improving model performance for credit card fraud detection.
