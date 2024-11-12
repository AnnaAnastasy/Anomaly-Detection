# Anomaly Detection for Credit Card Fraud

This project focuses on detecting fraudulent credit card transactions using anomaly detection methods. We apply and compare various algorithms, including **Isolation Forest**, **One-Class SVM**, **autoencoders**, **Local Outlier Factor**, and **DBSCAN**, to identify potentially fraudulent activities in credit card transaction data.

## Project Overview
Credit card fraud is a significant concern for financial institutions and customers. In this project, we employ machine learning techniques to build an anomaly detection model that flags potentially fraudulent transactions. This approach leverages the understanding that fraud cases are rare, thus fitting well within the scope of unsupervised learning for anomaly detection.

## Dataset
The dataset used in this project contains credit card transactions made by European cardholders in September 2013. The data represents transactions over a two-day period, where 492 transactions are identified as fraudulent out of a total of 284,807 transactions. This dataset is highly imbalanced, with the positive class (fraudulent transactions) making up only 0.172% of all entries.

- **Number of Transactions**: 284,807
- **Fraudulent Transactions**: 492
- **Class Imbalance**: Fraud transactions account for only 0.172% of total transactions

The dataset contains only numerical features that have been transformed using Principal Component Analysis (PCA) to protect confidentiality. Unfortunately, due to privacy concerns, no further information about the original transaction features is available.

## Project Structure
The project notebook includes the following sections:

- **Data Preprocessing**: Loading data, handling missing values, scaling, and preparing the data for model training.
- **Exploratory Data Analysis (EDA)**: Analyzing data distributions, correlations, and visualizations to understand fraud patterns.
- **Modeling**: Building, training, and evaluating multiple anomaly detection models.
- **Evaluation and Comparison**: Analyzing model performance using accuracy, precision, recall, and AUC-ROC scores.

## Methods Used
The following anomaly detection techniques were implemented and compared:

- **Isolation Forest**: Detects anomalies by isolating instances in feature space.
- **One-Class SVM**: Fits a boundary around the data points using support vector machine principles.
- **Autoencoder Neural Network**: Reconstructs normal transactions and flags deviations as anomalies.
- **Local Outlier Factor (LOF)**: Identifies samples that have significantly lower density than neighbors.
- **DBSCAN**: Density-based clustering used for outlier detection.
 
## Results
Each method’s performance is evaluated using metrics suited for anomaly detection, such as:

- Accuracy
- Precision
- Recall
- AUC-ROC
 
The best-performing model was identified based on these metrics, and insights into fraudulent transaction patterns were derived.

## Dataset Download Instructions
To run this project, you’ll need to download the credit card fraud detection dataset:

- Download the dataset from [Kaggle’s Credit Card Fraud Detection page](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).
- Save the downloaded `creditcard.csv` file in the same directory as the Jupyter Notebook (`anomaly-detection-credit-card-fraud.ipynb`).

## Setup and Installation

- Clone the repository:
```bash
  git clone https://github.com/AnnaAnastasy/Anomaly-Detection-Credit-Card-Fraud.git
```

- Navigate to the project directory:
```bash
  cd Anomaly-Detection-Credit-Card-Fraud
```

- Install required dependencies:
```bash
  pip install -r requirements.txt
```

- Launch Jupyter Notebook:
```bash
  jupyter notebook
```
Open `anomaly-detection-credit-card-fraud.ipynb` in the notebook interface.

## Usage
- Ensure the dataset file is located in the specified directory as indicated in the notebook.
- Run each cell sequentially in the notebook to preprocess the data, train models, and evaluate results.
- Adjust hyperparameters or try different algorithms as desired to observe changes in performance.

