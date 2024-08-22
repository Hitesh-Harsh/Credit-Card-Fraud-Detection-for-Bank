# Credit Card Fraud Detection Using LSTM RNN

## Overview
This project is aimed at detecting fraudulent credit card transactions using a Long Short-Term Memory (LSTM) Recurrent Neural Network (RNN). The dataset used for this project is synthetically generated through the BankSim Simulator, which mimics real banking transactions while maintaining the confidentiality required by financial institutions.

## Dataset
- **Source:** The dataset is generated using the BankSim Simulator.
- **Description:** The dataset represents transactions made by European cardholders, with each entry labeled as either fraudulent or non-fraudulent. It includes features that have been anonymized for privacy, including several categorical and numerical fields.
- **Balance:** The dataset is highly imbalanced, with a small percentage of transactions labeled as fraudulent.

## Data Preprocessing
Before training the model, extensive data preprocessing was performed:
1. **Data Cleaning:** Removed null values to ensure the dataset is clean and ready for analysis.
2. **Categorical Feature Transformation:** Converted categorical features into numeric values to make them suitable for model training.
3. **Handling Imbalance:** Applied Synthetic Minority Over-sampling Technique (SMOTE) to upsample the minority class (fraudulent transactions), balancing the dataset for more effective training.

## Model Training
The core of the project involves training an LSTM RNN model. The steps involved are:
- **Feature Scaling:** Normalized the features to ensure uniformity in the input data.
- **Model Architecture:** Constructed an LSTM RNN to capture temporal dependencies within the transaction data.
- **Training:** Trained the model on the preprocessed and upsampled dataset, optimizing it for the best performance in fraud detection.

## Results
The trained LSTM RNN model is evaluated using appropriate metrics, with an emphasis on precision, recall, and the F1 score due to the imbalanced nature of the dataset.
