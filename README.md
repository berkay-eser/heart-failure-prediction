
# Heart Disease Prediction Project

## Overview
This project aims to predict heart disease presence using various patient data features. The dataset containing information such as age, sex, chest pain type, resting blood pressure, cholesterol levels, and more. 

The project involves data preprocessing, exploratory data analysis (EDA), model building and training, and aims to deploy a model for practical use. Future steps include model improvement, creating a web application, developing a user-friendly interface, and enhancing documentation.


## Table of Contents
1. [Dataset](#dataset)
2. [Data Preprocessing](#data-preprocessing)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [Model Building and Training](#model-building-and-training)
5. [Usage](#usage)
6. [Results](#results)
7. [Contributing](#contributing)
8. [License](#license)

## Dataset
The dataset contains the following columns:
- ``Age``: Age of the patient
- ``Sex``: Sex of the patient ('M' for male, 'F' for female)
- ``ChestPainType``: Type of chest pain (e.g., ATA, NAP, ASY)
- ``RestingBP``: Resting blood pressure
- ``Cholesterol``: Cholesterol level
- ``FastingBS``: Fasting blood sugar (> 120 mg/dl, 1 = true; 0 = false)
- ``RestingECG``: Resting electrocardiogram results
- ``MaxHR``: Maximum heart rate achieved
- ``ExerciseAngina``: Exercise-induced angina ('Y' for yes, 'N' for no)
- ``Oldpeak``: ST depression induced by exercise relative to rest
- ``ST_Slope``: The slope of the peak exercise ST segment
- ``HeartDisease``: Indicator of heart disease (1 = presence, 0 = absence)

## Data Preprocessing
Data preprocessing steps included:
1. **Hangling Incorrect Values**: Some features contained incorrect values such as ``Cholesterol`` feature has value of 0 or ``RestingBP`` has value of 0. These values are not possible in a human being.
2. **Handling Missing Values**: Checked for any missing values and handled them appropriately.
3. **Encoding Categorical Features**: Converted categorical features into numerical features using ``OneHotEncoder()``.
4. **Splitting the Dataset**: Split the dataset into train and test sets.
5. **Feature Scaling**: Applied feature scaling to ensure all features contribute equally to the model training.

## Exploratory Data Analysis (EDA)
Performed EDA to understand the distribution and relationships between the features. Key steps included:
1. **Basic Informations About Dataset**: Checked missing values, data types, statistical values etc.
2. **Distribution of Numerical Features**: Checked distribution of numerical features for outliers.
3. **Data Imbalance Check**: Checked if target value is imbalanced.
4. **Visualizing Categorical Features Value Counts**: Visualizing categorical features with bar plot.

## Model Building and Training
The following steps were undertaken to build and train the model:
1. **Model Selection**: Selected appropriate machine learning algorithm (e.g., logistic regression, decision trees, random forest, etc.) by using cross-validation for recall metric.
2. **Hyperparameter Tuning**: Applied hyperparameter tuning to selected model by using GridSearchCV.
3. **Training**: Trained model using the training dataset.
4. **Evaluation**: Evaluated model performance using metrics such as accuracy, precision, recall, and F1-score on the test dataset.

## Results
The Random Forest Classifier model achieved the following performance metrics:
- **Accuracy**: 0.907
- **Recall**: 0.886
- **Precision**: 0.933
- **F1 Score**: 0.909
- **ROC-AUC**: 0.908

## Next Steps
The following steps are planned to further develop and enhance the project:
1. **Model Improvement**: Explore additional machine learning algorithms and techniques to improve model performance.
2. **Model Deployment**: Create an application for heart disease prediction using the trained model.
3. **User Interface**: Develop a user-friendly web interface for easy interaction with the prediction model.
4. **Documentation**: Enhance documentation to provide detailed usage instructions and examples.

These steps aim to refine the model, make it more accessible, and ensure its long-term usability and accuracy.

## Contributing
If you'd like to contribute, please fork the repository and use a feature branch. Pull requests are welcome.

## License
This project is licensed under the MIT License.
