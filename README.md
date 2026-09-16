# Advertising Sales Prediction

This project focuses on understanding how advertising expenditure through different channels affects sales. The dataset contains advertising spending on TV, Radio, and Newspaper along with the corresponding sales.

I used Python for data analysis and Linear Regression to study these relationships and build a model for predicting sales.

## Project Objective

The main objectives of this project are:

- Understand the relationship between advertising expenditure and sales.
- Analyze the effect of TV, Radio, and Newspaper advertising on sales.
- Build a Multiple Linear Regression model.
- Compare different feature combinations.
- Evaluate the models using R² Score and RMSE.
- Check the model using prediction error visualization.
- Study the interaction effect between TV and Radio advertising.

## Dataset

The dataset used in this project is `Advertising.csv`.

It contains the following columns:

- **TV** – Advertising expenditure through TV
- **radio** – Advertising expenditure through Radio
- **newspaper** – Advertising expenditure through Newspaper
- **sales** – Sales generated

Here, `sales` is the target variable.

## Technologies and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Scikit-learn
- Yellowbrick
- Jupyter Notebook

## Project Workflow

### 1. Data Loading

The dataset is loaded using Pandas and basic information about the data is explored.

### 2. Exploratory Data Analysis

Pair plots and a correlation heatmap are used to understand the relationship between the advertising features and sales.

### 3. Multiple Linear Regression

A Linear Regression model is trained using TV, Radio, and Newspaper as input features.

The regression coefficients are also calculated to understand the contribution of each feature to the model.

### 4. Feature Selection

Two models are compared:

- TV + Radio
- TV + Radio + Newspaper

The R² Score is used to compare the models. The models are compared to see whether adding Newspaper advertising provides a meaningful improvement.

### 5. Train/Test Evaluation

The dataset is divided into training and testing sets.

The models are evaluated using:

- **RMSE (Root Mean Squared Error)**
- **R² Score**

This helps in checking how the model performs on unseen test data.

### 6. Model Diagnostics

Yellowbrick's Prediction Error visualization is used to examine the model's prediction performance.

### 7. Interaction Effect

An additional feature is created by multiplying TV and Radio advertising:

`TV × Radio`

This interaction feature is added to the model to study whether the combined effect of TV and Radio advertising has an influence on sales.

## How to Run the Project

1. Download or clone this repository.
2. Keep `Advertising.csv` and `Advertising-Sales-Prediction.ipynb` in the same folder.
3. Open `Advertising-Sales-Prediction.ipynb` using Jupyter Notebook or Google Colab.
4. Run the cells in order.

## Repository Structure

```text
Advertising-Sales-Prediction/
│
├── Advertising-Sales-Prediction.ipynb
├── Advertising.csv
└── README.md
