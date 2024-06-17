# Vaccine Efficacy Prediction

This repository contains the implementation of a machine learning project aimed at predicting the efficacy of seasonal and XYZ vaccines. The project involves data cleaning, feature selection, model training, and evaluation using various probabilistic models.

## Table of Contents

- [Project Description](#project-description)
- [Data Preprocessing](#data-preprocessing)
  - [Data Cleaning and Imputation](#data-cleaning-and-imputation)
  - [File Segregation](#file-segregation)
  - [Feature Selection](#feature-selection)
- [Model Training](#model-training)
  - [Data Splitting](#data-splitting)
  - [Model Selection](#model-selection)
  - [Evaluation Metric](#evaluation-metric)
- [Final Submission](#final-submission)
- [Usage](#usage)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Project Description

This project aims to predict the efficacy of seasonal and XYZ vaccines using a dataset that has undergone extensive preprocessing and feature selection. Various probabilistic models were trained and evaluated, with Support Vector Machine (SVM) performing the best in terms of F1 score.

## Data Preprocessing

### Data Cleaning and Imputation

Data cleaning and imputation were performed simultaneously to ensure the dataset was ready for analysis. Missing values were handled appropriately to prevent any bias or inaccuracies in the model training process.

### File Segregation

The dataset was segregated into files for seasonal and XYZ vaccines. This segregation allows for training models specifically tailored to each type of vaccine, improving the accuracy and relevance of the predictions.

### Feature Selection

To select the most relevant features, the following methods were used:
- **Missing Value Threshold**: Features with a high percentage of missing values were removed.
- **Correlation Analysis**: Highly correlated features were identified and removed to prevent multicollinearity.
- **Chi-Square Test**: This test was used to select features that have a significant relationship with the target variable.

## Model Training

### Data Splitting

The dataset was split into three sets:
- **Train Set**: Used to train the models.
- **Test Set**: Used to evaluate the performance of the models.
- **Dev Set**: Used to detect and prevent overfitting during model training.

### Model Selection

Various probabilistic models were tested, with logistic regression serving as the baseline model. After extensive testing, SVM was found to perform the best among the tested models.

### Evaluation Metric

The F1 score was used as the main metric for model selection. The F1 score considers both precision and recall, providing a balanced measure of a model's performance.

## Final Submission

The probabilities from both the seasonal and XYZ vaccine models were combined to generate the final submission. This approach ensures that the predictions are comprehensive and accurate.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

