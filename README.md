## End to End Machine Learning Project
### Student Performance Indicator
An end-to-end machine learning project designed to predict and analyze student performance based on various features like parental education, test preparation, and demographic data. The goal is to identify key factors influencing academic outcomes.

### 📊 Dataset Overview
The dataset used for this project includes the following features:

##### Independent Variables:
Gender: Male/Female
Race/Ethnicity: Groups A, B, C, D, E
Parental Level of Education: High school, Associate's degree, Bachelor's degree, Master's degree, etc.
Lunch: Standard or free/reduced
Test Preparation Course: Completed/Not completed
Reading Score: Numeric score
Writing Score: Numeric score

##### Target Variable:
Math Score: Numeric score predicting student performance in mathematics.
Source: Kaggle - Students Performance in Exams

### Project Workflow
1. Data Ingestion
   Loaded data from CSV files.
   Split data into training and testing sets.
   Saved processed datasets for reuse using pipelines.
   
2. Exploratory Data Analysis (EDA)
   Explored relationships between features through visualizations.
   Identified correlations and key predictors of student performance.
   
3. Data Transformation
   Numeric Data:
     Handled missing values using the median strategy.
     Applied Standard Scaling for normalization.
   Categorical Data:
     Imputed missing values using the most frequent strategy.
     Applied One-Hot Encoding for categorical features.
     Scaled encoded data using Standard Scaling.
     Transformation pipelines were saved as .pkl files for efficient reuse.

4. Model Training
Evaluated multiple models; and selected the best one of them.
Applied hyperparameter tuning to optimize the model.
Exception handling was implemented to ensure robust model training and evaluation.
Saved the trained model as a .pkl file.

6. Deployment
Developed a Flask application to provide an interactive UI for predictions.
Integrated logging to monitor application and model performance.
Deployed the app on AWS EC2 Instance for public access.

### Technologies Used
Programming Language: Python
Libraries: Pandas, NumPy, Scikit-learn, Flask
Modeling: Tried Various models and selected the best one.
EDA: Matplotlib, Seaborn
Development Practices: Pipelines, Exception Handling, Logging
Deployment: Flask, AWS EC2 Instance
