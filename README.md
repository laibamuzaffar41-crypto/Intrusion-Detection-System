Intrusion Detection System using Machine Learning
Overview
This project presents a Machine Learning-based Intrusion Detection System (IDS) designed to identify malicious activities in network traffic. The system analyzes network connection data and classifies it as either normal or attack, enabling early detection of cyber threats.
The implementation is based on the NSL-KDD dataset, a widely used benchmark dataset for intrusion detection research.

Objectives
•	To build a classification model for detecting network intrusions
•	To compare the performance of multiple machine learning algorithms
•	To analyze which model performs best for intrusion detection tasks

Dataset
The project uses the NSL-KDD dataset, which contains labeled network traffic data including both normal and attack records.
Dataset Features:
•	Network-based features (e.g., duration, protocol type, bytes transferred)
•	Various attack types (DoS, Probe, R2L, U2R)
•	Labeled data for supervised learning

Methodology
1. Data Preprocessing
•	Removed unnecessary columns (e.g., difficulty level)
•	Converted categorical features into numerical format using one-hot encoding
•	Transformed labels into binary classes:
o	0 → Normal
o	1 → Attack
2. Data Splitting
•	Dataset divided into:
o	80% Training data
o	20% Testing data
3. Model Implementation
The following machine learning models were applied:
•	Logistic Regression
•	Decision Tree Classifier
•	Random Forest Classifier

Results
Model	Accuracy
Logistic Regression	95.2%
Decision Tree	99.84%
Random Forest	99.85%
Analysis
•	Random Forest achieved the highest performance
•	Ensemble learning helped improve accuracy and reduce overfitting
•	Decision Tree also performed well but is less stable compared to Random Forest

Evaluation Metrics
The models were evaluated using:
•	Accuracy
•	Precision
•	Recall
•	F1-Score
Recall is especially important in IDS, as it measures the ability to correctly detect attacks.

Conclusion
This project demonstrates that machine learning techniques can effectively detect network intrusions. Among the tested models, Random Forest provided the best performance due to its ensemble nature and robustness.



