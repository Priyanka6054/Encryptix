# Credit Card Fraud Detection
## Project Overview
This project focuses on detecting fraudulent credit card transactions using machine learning techniques. Given the highly imbalanced nature of the dataset, special attention is paid to handling class imbalance while training the model.
## Dataset Overview
The dataset used in this project is the https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud dataset. It contains transactions made by credit cards in September 2013 by European cardholders. The dataset presents transactions that occurred over two days, with 492 frauds out of 284,807 transactions.
* Number of Instances: 284,807
* Number of Features: 30
  - The features V1, V2, ..., V28 are the principal components obtained with PCA.
  - The only features which have not been transformed with PCA are Time and Amount.
  - Feature Time contains the seconds elapsed between this transaction and the first transaction in the dataset.
  - Feature Amount is the transaction amount.
  - Feature Class is the response variable and it takes value 1 in case of fraud and 0 otherwise.
## Project Structure
The project is organized as follows:
### 1. Data Collection:
- Loading the dataset using Pandas.
- Initial exploration to understand the data structure and check for null values.
### 2. Data Preprocessing
- Handling missing values: Checking for any missing values and handling them accordingly. In this dataset, there are no missing values.
- Descriptive statistics: Reviewing summary statistics of the dataset.
### 3. Feature Scaling
- Scaling features: Scaling features Time and Amount using StandardScaler as they are not transformed by PCA.
### 4. Data Splitting
- Splitting the dataset: Using train_test_split to split the dataset into training and testing sets.
### 5. Handling Class Imbalance
- Addressing class imbalance: Using techniques such as RandomOverSampler and RandomUnderSampler from the imblearn library.
### 6. Model Training
- Training a RandomForestClassifier: Building and training the model.
- Evaluating the model: Using various metrics such as accuracy, precision, recall, F1 score, and confusion matrix.
### 7. Model Evaluation
- Visualizing the performance: Using confusion matrix plots.
- Calculating metrics: Assessing the model's performance on the test data.
### 8. Visualization
- Presenting the results: Using graphs and charts for better understanding and interpretation.
  
## Libraries Used
* pandas
* numpy
* scikit-learn
* matplotlib
* seaborn
* imbalanced-learn (imblearn)

## Results
* The final model's performance is summarized in terms of accuracy, precision, recall, and F1 score.
* Confusion matrix visualizations provide insights into the classification results.

## Conclusion
The project successfully demonstrates the process of building a machine learning model to detect fraudulent credit card transactions, with a particular focus on handling imbalanced data. Future work could explore other advanced techniques and models to improve detection performance.



