# Credit-Card-Fraud-Detection

This project demonstrates a machine learning model to detect fraudulent credit card transactions using a logistic regression model. The dataset is heavily imbalanced, so techniques like SMOTE (Synthetic Minority Over-sampling Technique) are used to oversample the minority (fraud) class. The project includes data preprocessing, scaling, oversampling, training, evaluation, and visualization of the model's performance.

## Table of Contents
- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Evaluation](#model-evaluation)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The goal of this project is to build a machine learning model that can detect fraudulent credit card transactions. The project involves:
- Loading and preprocessing the data.
- Addressing the class imbalance using SMOTE.
- Training a logistic regression model to classify transactions as fraudulent or non-fraudulent.
- Evaluating the model using accuracy, precision, recall, and F1-score metrics.

## Technologies Used
- **Python**: Version 3.x
- **Pandas**: For data manipulation and analysis
- **Scikit-learn**: For machine learning models and evaluation metrics
- **Imbalanced-learn**: For oversampling techniques (SMOTE)
- **Matplotlib**: For data visualization

## Dataset
The dataset used in this project is a **credit card transaction dataset** (`creditcard.csv`) which contains transactions labeled as either fraudulent (`Class=1`) or non-fraudulent (`Class=0`). It is highly imbalanced, with only a small percentage of fraudulent transactions.

- **Features**: 
  - Time, Amount, and 28 anonymized features (V1, V2, ..., V28)
  - Target variable: `Class` (1 for fraud, 0 for non-fraud)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/aisha-gama/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
2. Install the required dependencies:
   
   ```bash
   pip install -r requirements.txt

3. Download the dataset and place it in the root directory of the project. The dataset should be named creditcard.csv.

## Usage
After cloning the repository and setting up the environment, follow the steps below to run the project:
**Preprocess the data**: This includes loading the data, scaling the Amount feature, and oversampling using SMOTE.
**Train the model**: The logistic regression model is trained on the resampled data.
**Evaluate the model**: After training, the model is tested, and evaluation metrics such as accuracy, precision, recall, and F1-score are calculated.
**Visualize the results**: A bar chart is generated to compare precision, recall, and F1-scores between the two classes.
   
## Model Evaluation
The model is evaluated using the following metrics:
- **Accuracy**: Overall performance of the model.
- **Precision**: The ratio of true positives to the sum of true and false positives.
- **Recall**: The ratio of true positives to the sum of true positives and false negatives.
- **F1-Score**: The harmonic mean of precision and recall.
- A bar chart is generated to visualize the comparison of precision, recall, and F1-scores between non-fraudulent and fraudulent classes.

## Contributing
Contributions are welcome! If you'd like to contribute to this project, please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

