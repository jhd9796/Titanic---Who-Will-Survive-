# Titanic: Who Will Survive?

## Overview
This project explores the tragic event of the Titanic's sinking, focusing on predicting which passengers survived based on various features. Utilizing machine learning algorithms, we delve into the socio-economic status, age, gender, and family size of passengers to uncover patterns and factors contributing to the likelihood of survival.

## Data Source
The dataset comprises two main files: `train.csv` and `test.csv`, which include passenger details such as Age, Sex, Passenger Class (Pclass), and Survival status, among others. The training set was used to build the machine learning models, while the test set helped evaluate their performance.

## Methodology
We began by cleaning the data, addressing missing values and outliers, particularly in the 'Age' and 'Cabin' columns. K-Nearest Neighbors (KNN) imputation was applied to fill in missing age values, considering its advantage over mean imputation due to the significant amount of missing data.

Key features were analyzed to understand their impact on survival rates. We explored relationships between socio-economic status, age, gender, and family size on board. Machine learning models employed include:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Random Forest Classifier

Each model was trained on the dataset and evaluated based on accuracy, precision, recall, and F1 scores. Cross-validation further assessed the models' effectiveness, and Receiver Operating Characteristic (ROC) curves were plotted to compare their performance comprehensively.

## Findings
The analysis revealed that gender, class, and fare were highly correlated with survival chances. Our models showed that logistic regression, with the highest Area Under the Curve (AUC) value, outperformed the other models, making it the most suitable for predicting survival on the Titanic.

## Installation
To run this project, you will need Python along with libraries like pandas, numpy, matplotlib, seaborn, and scikit-learn. Install these using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage
You can replicate our findings or explore the dataset further by running the Jupyter notebook included in this repository. Ensure you have Jupyter installed:

```bash
pip install notebook
```

To start the notebook:

```bash
jupyter notebook Titanic-Who_Will_Survive.ipynb
```
