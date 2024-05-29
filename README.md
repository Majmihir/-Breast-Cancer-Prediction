# Breast Cancer Prediction Using Support Vector Machine (SVM)

## Project Description

This project aims to develop a machine learning model to predict breast cancer using the Breast Cancer Wisconsin (Diagnostic) dataset. The primary objective is to classify tumors as malignant or benign based on various features derived from fine needle aspirate (FNA) of breast mass. The project is divided into three main phases: Data Preprocessing, Feature Selection and Engineering, and Machine Learning Model implementation.

## Data Sources
Breast cancer data: The primary dataset used for this analysis is Kaggel Breast Cancer Wisconsin (Diagnostic) dataset "Breast_cancer.csv" file, containing detailed information about  whether the cancer is benign(
B) or malignant(M).

## Project Phases

### 1. Data Preprocessing
Objective: Clean and preprocess the Breast Cancer Wisconsin (Diagnostic) dataset to ensure high-quality input for the machine learning model.
#### Tasks:
Handle missing values by imputing or removing them.
Identify and treat outliers to ensure they do not adversely affect the model.
Resolve any other inconsistencies in the data to maintain data integrity.
#### Documentation:
Missing Values: Missing values were handled by removing rows with missing entries.
#### Outliers: 
Outliers were identified using box plots and statistical methods. Extreme outliers were treated or removed to prevent skewing the model.

![density_graph](https://github.com/Majmihir/-Breast-Cancer-Prediction/assets/110147459/e51ee89a-fd55-4eb9-8594-4ff486d7d1f3)

#### Normalization: 
Features were normalized to ensure they are on a similar scale, which helps in improving the model performance.
### 2. Feature Selection and Engineering
#### Objective:
Identify and engineer relevant features to improve the model's predictive performance.
#### Tasks:
Analyze and select the most significant features from the dataset.
Create new features or transformations that might enhance the model's ability to distinguish between malignant and benign tumors.
#### Documentation:
Feature Selection: Relevant features were selected using correlation analysis and feature importance from preliminary models.
Feature Engineering: New features were created based on domain knowledge and statistical transformations (e.g., polynomial features, interaction terms).

![correaltion](https://github.com/Majmihir/-Breast-Cancer-Prediction/assets/110147459/77d2c263-0611-4ead-9d8d-2f4679ab03c7)

### 3. Machine Learning Model (SVM)
#### Objective: 
Implement and evaluate a Support Vector Machine (SVM) model for breast cancer prediction.
#### Tasks:
Develop an SVM model to classify tumors into malignant or benign categories.
Train the SVM model using the preprocessed dataset.
Evaluate the model's performance using appropriate metrics such as accuracy, precision, recall, and F1-score.


### Additional Models Tested:

### Linear Regression:
Tested but found less effective due to the nature of classification problem.

### Decision Tree Classifier:
Provided reasonable results but was prone to overfitting.

### K-Nearest Neighbors (KNN): 
Showed good performance but was computationally expensive with larger datasets.

### SVM Model:
Gave the best results in terms of accuracy and overall performance.

### Documentation:
Model Training: The SVM model was trained on the dataset using a radial basis function (RBF) kernel.

#### Model Evaluation:
The model was evaluated using cross-validation to ensure robustness. Performance metrics included accuracy, precision, recall, and F1-score.

![PE_breast_cancer](https://github.com/Majmihir/-Breast-Cancer-Prediction/assets/110147459/87675273-d8de-4407-8ed5-3d8c0e01f8f5)


#### ROC Curve Comparison:
ROC curves for each model (Linear Regression, Decision Tree, KNN, and SVM) were plotted and compared. The SVM model demonstrated the best performance with the highest area under the ROC curve (AUC).


![roc_breast_cancer](https://github.com/Majmihir/-Breast-Cancer-Prediction/assets/110147459/87741415-dda1-4fdb-be5c-ef5b74871d41)
