# Intrusion-Detection
This project focuses on building an Intrusion Detection System (IDS) for Software-Defined Networking (SDN) using machine learning techniques. The system is designed to detect various types of network attacks by analyzing the NSL-KDD dataset. Two models, Support Vector Machine (SVM) and Artificial Neural Network (ANN), were trained and evaluated to detect and classify network intrusions.





Intrusion detection system for SDN

	Dataset: NSL-KDD (train & test data set)
•	Added column to dataset.


	Data Cleaning:
•	There are not any null values in the dataset of train and test dataset.


	Data Pre-processing:
•	Attack column in the dataset is merged to form attack_categories. It is the target variable in the dataset.

•	Classifying each attack to attack type. The different attack types are:

o	Denial of Service attacks

o	Probe attacks

o	Privilege escalation attacks

o	Remote access attacks


	Data Visualization:
•	Bar plot for attack category.

•	Analyze the target variable with features.

	Encoding:
•	Changed the Object types in the train and test dataset and encoded them.


	Feature Selection: 
•	Heatmap is plotted.

•	Finding features that are highly correlated (correlation coefficient > 0.5) with 'attack_category'.

•	Finding features that are low correlated (correlation coefficient < 0.1) with 'attack_category'.

•	Dropped the highly correlated and low correlated features with attack_category.

	Feature Scaling.
•	Standard Scaler is used for feature scaling, for normalizing the features.

	Model Training:
•	SVM

o	Overall Accuracy is 98%.

o	However, accuracy alone may not be sufficient for evaluating the model’s performance.

o	Confusion Matrix is plotted for more detailed information about the model’s performance.

o	Overall, the SVM model demonstrates strong performance for most classes, with high precision, recall, and F1-scores. However, it struggles with class 0, where the recall is relatively low, indicating that the model misses a significant portion of the actual instances.

•	ANN
o	Overall, the ANN model demonstrates strong performance, with high accuracy and precision-recall values for most classes. However, like the SVM model, it struggles with class 0, where the recall is relatively low, indicating that the model misses a significant portion of the actual instances.
