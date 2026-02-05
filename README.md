

---

# Forest Fires Machine Learning Project

This project uses machine learning to **predict the Fire Weather Index (FWI)** based on environmental and weather features related to forest fires.

FWI (Fire Weather Index) is a metric that estimates wildfire risk using weather conditions such as temperature, humidity, wind speed, and rainfall.

## Project Overview

Forest fires are destructive and difficult to predict. This project trains regression models on historical fire and weather data so that, given environmental inputs, the system can estimate the FWI — a proxy for fire potential and severity.

## Dataset

The dataset contains:

* Temperature
* Relative humidity
* Wind speed
* Rainfall
* Fire weather indices (FFMC, DMC, DC, ISI)
* Fire Weather Index (FWI) — target variable

The goal is to train a model that predicts FWI from the other features.

## Machine Learning Pipeline

1. Load and preprocess data
2. Perform exploratory data analysis
3. Scale/standardize features
4. Train regression models (e.g., Linear Regression, Lasso, Ridge, Elastic Net)
5. Evaluate model performance
6. Save the best trained model for inference

## Models Used

* Linear Regression
* Ridge Regression
* Lasso Regression
* Elastic Net Regression

Regularization techniques help reduce overfitting and improve prediction reliability.

## Challenges and Solutions

**Data scaling:**
Features have different scales. Solution: feature standardization.

**Model overfitting:**
Linear regression alone can overfit. Solution: use regularized models like Ridge and Lasso.

**Model validation:**
Solution: use cross-validation to tune hyperparameters and evaluate performance.

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/rohithsukka/forest-fires.git
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the application:

```bash
python application.py
```

4. After the server starts, open your browser and go to:

```
http://localhost:5000/predictdata
```

This will show the FWI predictions based on input variables.

## Technologies Used

* Python
* pandas
* NumPy
* scikit-learn
* Flask (for web app)
* Matplotlib / Seaborn (for visualizations)

## Outcome

The trained regression model predicts the Fire Weather Index (FWI) given environmental inputs. This helps estimate forest fire risk based on current weather conditions.
