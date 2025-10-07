🫀 Heart Disease Prediction Project
Overview
This project focuses on building and evaluating machine learning models to predict the presence of heart disease based on various clinical and demographic features. The goal is to provide a comprehensive analysis of the dataset, including exploratory data analysis (EDA), data preprocessing, and model comparison.

💾 Dataset
The analysis uses a Heart Disease Dataset (heart_disease_dataset.csv).


Dataset Quick Facts

Total Entries: 303.



Columns: 14 (features + target variable).



Data Types: All columns are numerical (1 float64 and 13 int64).



Missing Values: There are no missing values in the dataset, which simplifies the data cleaning process.





Target Variable: output (0: No Heart Disease, 1: Yes Heart Disease).


📊 Exploratory Data Analysis (EDA) Highlights
Age Distribution
The distribution of age in the dataset is visualized in a histogram, helping to understand the age range of the patients.


Key Feature Visualizations

Cholesterol vs. Blood Pressure: A scatter plot was used to visualize the relationship between 'chol' (Cholesterol) and 'trtbps' (Blood Pressure).



Average Age by Heart Disease: A bar plot compared the average age of patients with and without heart disease.



Cholesterol Distribution by Heart Disease: A boxplot showed the distribution of 'chol' for patients with and without heart disease.


Correlation Matrix: A heatmap was generated to visualize the correlation between all features.

⚙️ Data Preprocessing
As all columns were found to be numerical and there were no missing values, the dataset was immediately ready for modeling.


Missing Values: Confirmed to be zero across all features.



Categorical Encoding: The one-hot encoding step was skipped as there were no object type columns (categorical features) in the dataset.




Scaling: Standard Scaling was applied to the features before training the final Logistic Regression model to potentially improve performance.


Splitting: The data was split into training and testing sets with a 20% test size.


Training Set Size (X_train): (242,13).


Test Set Size (X_test): (61,13).

🧠 Model Training and Evaluation
We evaluated the performance of two popular classification algorithms: Logistic Regression and Random Forest Classifier.

1. Logistic Regression (Initial)
Metric	Score
Accuracy	
0.8033 

Precision	
0.7692 

Recall	
0.9091 

F1-score	
0.8333 


Export to Sheets
2. Random Forest Classifier
Metric	Score
Accuracy		
0.8361 


Precision	
0.7805 


Recall		
0.9697 


F1-score		
0.8649 



Export to Sheets
3. Logistic Regression (Scaled Data)
The model was retrained after applying Standard Scaling to the features.

Metric	Score
Accuracy	
0.8361 


Precision		
0.7879 


Recall	
0.7879 


F1-score	
0.7879 



