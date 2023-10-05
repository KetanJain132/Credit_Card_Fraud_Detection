# Credit Card Fraud Detection

## Introduction

Credit card fraud is a significant concern in the financial industry, with billions of dollars lost each year due to fraudulent transactions. This project focuses on developing a credit card fraud detection system using machine learning techniques.

## Data Preprocessing

The initial steps of data preprocessing include:

- Converting the 'Fraud' column into a factor with levels 0 and 1.
- Removing unnecessary columns from the dataset.
- Handling missing values in the 'Zip' column by replacing them with the mean value.

## Exploratory Data Analysis

The exploratory data analysis phase involves:

- Checking for missing values, which are handled as mentioned above.
- Providing a summary of the dataset to gain insights into its distribution.
- Visualizing the distribution of fraud and non-fraud transactions using bar plots.

## Data Splitting

The dataset is divided into a training set and a test set using random sampling. The `caret` library is used for this purpose.

## Model Building

### Random Over-sampling and Random Under-sampling

Both random over-sampling and random under-sampling techniques are applied to balance the dataset. This helps to address the issue of class imbalance.

#### Random Over-sampling

- Random over-sampling increases the number of instances in the minority class (fraud).
- A random forest classifier is trained on the over-sampled data.
- Predictions are made on the test dataset.
- Model performance is evaluated using a confusion matrix.

#### Random Under-sampling

- Random under-sampling reduces the number of instances in the majority class (non-fraud).
- A random forest classifier is trained on the under-sampled data.
- Predictions are made on the test dataset.
- Model performance is evaluated using a confusion matrix.

### Random Over-sampling

Random over-sampling increases the number of instances in the minority class (fraud). The steps include:

- Performing random over-sampling to balance the dataset.
- Training a random forest classifier.
- Making predictions on the test dataset.
- Evaluating model performance using a confusion matrix.

## Conclusion

Credit card fraud detection is a critical application of machine learning. By applying techniques such as random over-sampling and random under-sampling, we can improve the detection of fraudulent transactions and reduce financial losses.

Please note that this readme provides an overview of the project and does not include the actual code. Refer to the code file for implementation details.
