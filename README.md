
[![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)

## Overview

This project aims to predict **customer churn** for a telecom company using various machine learning models. Customer churn occurs when customers stop doing business with a company, and predicting churn helps companies take proactive measures to retain customers.

---

## Process Flow

The general workflow for this project is as follows:

### 1. Data Preprocessing Flow

![Data Preprocessing Flow](/mnt/data/A_flowchart_visualizing_data_preprocessing_for_mac.png)

- Handle missing values.
- Convert categorical variables to numeric using Label Encoding.
- Check for multicollinearity and remove highly correlated features using VIF.

### 2. Model Building Flow

![Model Building Flow](/mnt/data/A_flowchart_visualizing_model_building_steps_for_a.png)

- Split the dataset into training and testing sets.
- Train multiple machine learning models.
- Evaluate models using metrics such as accuracy, confusion matrix, and more.

---

## Dataset

The dataset contains customer information such as demographic details, services subscribed, billing information, and whether the customer churned or not. Key columns include:

  - **customerID**: Unique identifier for each customer.
  - **gender**: Gender of the customer.
  - **SeniorCitizen**: Whether the customer is a senior citizen (1 for Yes, 0 for No).
  - **Partner**: Whether the customer has a partner.
  - **Dependents**: Whether the customer has dependents.
  - **tenure**: Number of months the customer has stayed with the company.
  - **PhoneService**: Whether the customer has a phone service.
  - **InternetService**: Type of internet service (DSL, Fiber optic, No).
  - **Churn**: Target variable indicating if the customer churned (Yes/No).
  
---

## Project Structure
  
  - **data/**: Directory containing the dataset (`customer_churn.csv`).
  - **notebooks/**: Jupyter notebooks with data exploration, preprocessing, and model training.
  - **models/**: Directory to save trained models.

---

## Usage

1. **Data Preprocessing**:
    - Handle missing values.
    - Convert categorical variables into numeric form using Label Encoding.
    - Check for multicollinearity using Variance Inflation Factor (VIF) and remove highly correlated features.
  
2. **Model Building**:
    - Split the dataset into training and testing sets.
    - Train and evaluate Logistic Regression, Decision Tree, and Random Forest models.
    - Measure model performance using accuracy scores.
  
3. **Feature Engineering**:
    - Experiment with feature selection and engineering to improve model performance.
  
4. **Evaluation**:
    - Evaluate the models using accuracy, confusion matrix, and other relevant metrics.
    - Compare the performance of different models.

---

## Results

- **Logistic Regression**: Achieved an accuracy of 76.7%.
- **Decision Tree**: Achieved an accuracy of 73.0%.
- **Random Forest**: Achieved an accuracy of 76.8%.

The Random Forest model performed the best, making it a strong candidate for predicting customer churn.

---

## Future Work

- Experiment with more advanced models like XGBoost.
- Perform hyperparameter tuning to further improve model performance.
- Analyze feature importance to understand which features contribute most to churn prediction.

---

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to create a pull request or open an issue.

---

## Acknowledgements

- [Pandas Documentation](https://pandas.pydata.org/docs/index.html)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Seaborn Documentation](https://seaborn.pydata.org/)
