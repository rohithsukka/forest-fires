---

# Forest Fires Prediction and Analysis

This project focuses on analyzing and predicting forest fire behavior using machine learning techniques and environmental data.

## Project Overview

Forest fires cause serious environmental and economic damage. This project uses historical forest fire data along with weather and environmental features to build machine learning models that help understand fire behavior and predict the extent of fire damage.

The main objective is to train regression models to predict the **burned area** of forest fires based on input features such as temperature, humidity, wind speed, and weather indices.

## Dataset

The dataset contains meteorological and environmental attributes related to forest fires, including:

* Temperature
* Relative humidity
* Wind speed
* Rainfall
* Fire weather indices (FFMC, DMC, DC, ISI)
* Burned area (target variable)

## Project Workflow

1. Data loading and preprocessing
2. Exploratory data analysis
3. Feature scaling and transformation
4. Model training using regression techniques
5. Model evaluation and comparison
6. Saving trained models for reuse

## Machine Learning Models Used

* Linear Regression
* Ridge Regression
* Lasso Regression
* Elastic Net Regression

Regularization techniques were applied to reduce overfitting and improve model generalization.

## Challenges Faced

* Features had different scales, affecting model performance
* Overfitting in basic regression models
* Selecting the right evaluation metrics

## How Challenges Were Addressed

* Applied feature scaling using standardization
* Used regularization methods (Ridge, Lasso, Elastic Net)
* Performed cross-validation for model tuning and validation

## Results

Regularized regression models performed more consistently than basic linear regression. The models helped identify important factors influencing forest fire behavior, such as temperature, humidity, and wind speed.

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## How to Run the Project

1. Clone the repository

```bash
git clone https://github.com/rohithsukka/forest-fires.git
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Run the notebooks or application file

```bash
python application.py
```

## Key Learnings

* Importance of data preprocessing and feature scaling
* Practical understanding of regression and regularization
* Model evaluation using real data behavior
* Building an end-to-end machine learning workflow


