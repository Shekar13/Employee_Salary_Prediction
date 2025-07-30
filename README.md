# Employee Salary Prediction

This project focuses on predicting employee monthly salaries using various machine learning regression models. The goal is to build a predictive model and deploy a user-friendly interface for interactive salary predictions.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Models Used](#models-used)
- [Results](#results)
- [Web Interface](#web-interface)
- [Future Scope](#future-scope)
- [References](#references)
- [License](#license)

## Project Overview

This project implements a machine learning pipeline to predict employee monthly salaries. It covers data loading, preprocessing, exploratory data analysis, training multiple regression models, evaluating their performance, and deploying a simple web interface using Gradio for interactive predictions.

## Dataset

The dataset used for this project is `employee.csv`. It contains various employee-related features that influence their monthly salary.

## Features

The dataset includes the following features:
* `Employee ID`
* `Department`
* `Gender`
* `Age`
* `Job Title`
* `Hire Date`
* `Years At Company`
* `Education Level`
* `Performance Score`
* `Monthly Salary`
* `Work Hours Per Week`
* `Projects Handled`
* `Overtime Hours`
* `Sick Days`
* `Remote Work Frequency`
* `Team Size`
* `Training Hours`
* `Promotions`
* `Employee Satisfaction Score`
* `Resigned`

## Installation

To set up the project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/employee-salary-prediction.git](https://github.com/yourusername/employee-salary-prediction.git)
    cd employee-salary-prediction
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate # On Windows use `venv\Scripts\activate`
    ```

3.  **Install the required libraries:**
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn joblib xgboost gradio
    ```

## Usage

You can run the Jupyter Notebook (`EmployeeSalaryPrediction.ipynb`) to see the full analysis, model training, and evaluation steps. To launch the Gradio web interface, execute the relevant Gradio interface setup code within the notebook or as a separate Python script after saving the trained model.

## Models Used

The project explored the following regression models:
* **Linear Regression**: A basic linear model.
* **Random Forest Regressor**: An ensemble learning method providing high accuracy.
* **XGBoost Regressor**: A powerful gradient boosting framework.

## Results

* **Linear Regression:**
    * [cite_start]MSE: 16186.224025 [cite: 1]
    * [cite_start]R2 Score: 0.99140 [cite: 1]
* **Random Forest Regressor:**
    * [cite_start]MSE: 6.8 [cite: 1]
    * [cite_start]R2 Score: 1.0 [cite: 1]
* **XGBoost Regressor:**
    * [cite_start]MSE: 29.6593475348 [cite: 1]

The Random Forest model achieved exceptional accuracy, suggesting a strong fit to the dataset.

## Web Interface

A simple web interface is built using Gradio, allowing users to input employee details and receive an instant salary prediction. This interface facilitates easy interaction with the trained model.

## Future Scope

* **Model Improvement:** Explore advanced models (Deep Learning), fine-tune existing ones, and use cross-validation for better accuracy and reliability.
* **Data Enrichment:** Integrate external (economic, industry) and more detailed internal data (performance reviews).
* **Deployment & Maintenance:** Develop a robust web app, automate deployment with CI/CD, and continuously monitor model performance in production.

## References

* [cite_start]`EmployeeSalaryPrediction.ipynb - Colab.pdf` (Original project notebook/document) [cite: 1]

## License

This project is licensed under the MIT License - see the `LICENSE` file for details (You should create a LICENSE file in your repo).
