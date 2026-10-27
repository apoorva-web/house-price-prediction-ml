# house-price-prediction-ml
A beginner-friendly machine learning project that predicts house prices using property characteristics such as area, location, property type, BHK, and age. Built with Python, Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn.
# House Price Prediction Using Machine Learning

## Project Overview

This project uses Machine Learning to predict house prices based on different property characteristics.

The dataset contains **80,000 property records** with information about property size, location, number of bedrooms, bathrooms, property age, and other features.

The project uses **Linear Regression** to estimate property prices. It also explores the dataset through data analysis and visualizations to better understand the factors associated with house prices.

## Objectives

- Explore and understand the housing dataset.
- Perform exploratory data analysis (EDA).
- Visualize numerical features and their distributions.
- Study correlations between numerical features and house prices.
- Convert categorical features into numerical values.
- Train a Linear Regression model.
- Evaluate model performance using standard regression metrics.
- Compare actual house prices with predicted prices.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Dataset Features

The dataset includes the following types of information:

| Feature | Description |
|---|---|
| City | City in which the property is located |
| Locality_Type | Locality category, such as Affordable, Mid-Range, or Premium |
| Property_Type | Type of property, such as Apartment, Villa, or Independent House |
| BHK | Number of bedrooms, hall, and kitchen configuration |
| Bathrooms | Number of bathrooms |
| Super_Area_SqFt | Super built-up area in square feet |
| Carpet_Area_SqFt | Carpet area in square feet |
| Floor_Number | Floor on which the property is located |
| Total_Floors | Total floors in the building |
| Age_of_Property | Age of the property |
| Furnishing_Status | Furnishing category |
| Parking | Parking availability indicator |
| Lift_Available | Lift availability indicator |
| Gated_Community | Whether the property is in a gated community |
| Distance_to_Metro_km | Distance to the nearest metro in kilometres |
| Distance_to_City_Center_km | Distance to the city centre in kilometres |
| Price_INR_Lakhs | Target variable: property price in lakhs of Indian rupees |

`Property_ID` is an identifier and is excluded from the final model.

## Project Workflow

### 1. Data Exploration
- Examined the dataset's shape, columns, and data types.
- Viewed descriptive statistics.
- Checked for missing values and duplicate records.

### 2. Exploratory Data Analysis
- Created histograms to understand numerical feature distributions.
- Used count plots to examine selected categorical or binary features.
- Used box plots to inspect potential outliers.
- Examined correlations between numerical variables.

### 3. Data Preprocessing
- Prepared the input features and target variable.
- Converted categorical features into numerical columns using one-hot encoding.
- Excluded the property identifier from the final model.
- Applied a logarithmic transformation to the target price to help handle its skewed distribution.

### 4. Model Training
- Used Linear Regression as the prediction algorithm.
- Split the data into training and testing sets.
- Used an 80:20 train-test split with `random_state=42`.

### 5. Model Evaluation
Evaluated the model using:
- R² Score
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

A comparison table was also created to examine actual and predicted house prices.

## Model Performance

The final Linear Regression model produced the following results:

| Metric | Result |
|---|---:|
| R² Score | 0.7484 |
| Mean Absolute Error (MAE) | ₹34.82 lakhs |
| Root Mean Squared Error (RMSE) | ₹74.63 lakhs |

The R² score indicates that the model explains approximately 74.84% of the variance in the test-set house prices, based on the evaluation procedure used.

The MAE indicates an average absolute prediction error of approximately ₹34.82 lakhs. The RMSE penalizes larger errors more heavily, so its higher value suggests that some predictions have relatively large errors.

**Note:** These are the results from the final model in the notebook. They do not guarantee the same performance on new properties or real-world market data.

## How to Run the Project

### Step 1: Clone the repository

```bash
git clone <your-repository-url>
```

### Step 2: Open the project folder

```bash
cd house-price-prediction-ml
```

### Step 3: Install the required libraries

```bash
pip install -r requirements.txt
```

### Step 4: Open Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the notebook

Open `house_pricing.ipynb` and run the cells in order.

Ensure that `house_pricing.csv` is in the same folder as the notebook.

## Project Structure

```text
house-price-prediction-ml/
│
├── house_pricing.ipynb
├── house_pricing.csv
├── requirements.txt
└── README.md
```

## Limitations

- The project currently uses Linear Regression.
- Prediction errors can be substantial for individual properties.
- The reported results depend on the dataset and train-test split.
- The model has not been demonstrated to be a production-ready house valuation system.
- Further testing with alternative algorithms and unseen data is needed.

## Future Improvements

- Compare Linear Regression with Random Forest and other regression algorithms.
- Improve feature engineering and preprocessing.
- Analyze prediction errors across different price ranges and cities.
- Tune model parameters and compare evaluation metrics.
- Build a simple user interface that accepts property details and displays a predicted price.

## Conclusion

This project demonstrates a complete beginner-level machine learning workflow, from exploring and preparing a dataset to training a regression model and evaluating its predictions.

It provides a foundation for further learning in data analysis, feature engineering, regression, and model evaluation.

## Author

Created as a machine learning learning project.
