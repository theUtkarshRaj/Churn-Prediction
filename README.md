---
# Churn Prediction

This project aims to predict customer churn in a bank using Deep Learning learning. The model takes various customer data features as inputs, such as demographics, account balance, and activity, to predict the likelihood of churn. This prediction helps banks identify customers who are at risk of leaving, allowing them to take proactive steps to retain valuable clients.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Data Preprocessing](#data-preprocessing)
4. [Model](#model)
5. [Deployment](#deployment)
6. [Installation](#installation)
7. [Usage](#usage)
8. [License](#license)

## Project Overview

This Churn Prediction model is trained on a dataset containing customer information, including factors like age, balance, and tenure. After preprocessing and training, the model can classify whether a customer is likely to churn or stay. A Streamlit application is included to provide an interactive user interface for predictions.

## Features

- **Data Preprocessing**: Cleans and transforms raw data using one-hot encoding and standard scaling.
- **Label Encoding**: Encodes categorical data such as `Gender` and `Geography`.
- **Model Training**: Uses a TensorFlow-based model to train on customer data and predict churn.
- **Interactive Interface**: A Streamlit app allows users to input customer data and view churn predictions.
  
## Data Preprocessing

The preprocessing steps include:

1. Encoding categorical features (`Gender`, `Geography`).
2. Scaling numeric features (`CreditScore`, `Balance`, `EstimatedSalary`, etc.).
3. Preparing data to match the input format of the machine learning model.

## Model

The model is a neural network built with TensorFlow and trained on customer data. It takes in features like credit score, balance, age, and encoded values for geography and gender, and outputs the probability of churn.

## Deployment

The project includes a **Streamlit app** for easy deployment and user interaction. With Streamlit, you can:

- Enter customer details through a simple form.
- Receive immediate predictions on the likelihood of churn.
  
## Installation

To run the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/theUtkarshRaj/Churn-Prediction.git
   cd Churn-Prediction
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## Usage

1. Launch the Streamlit app following the [Installation](#installation) instructions.
2. Input customer details such as `Geography`, `Gender`, `Credit Score`, `Balance`, etc.
3. Click **Submit** to get a churn prediction result.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---
