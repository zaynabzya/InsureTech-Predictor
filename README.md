# Insurance Cost Prediction

## Overview
This project predicts insurance costs using machine learning models based on demographic and health-related data. It involves data cleaning, preprocessing, exploratory data analysis (EDA), model training, evaluation, and model comparison.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Models](#models)
- [Results](#results)
- [Contributing](#contributing)


## Installation
To run the project, follow these steps:

```bash
git clone https://github.com/yourusername/insurance-cost-prediction.git
cd insurance-cost-prediction
pip install -r requirements.txt
```

# Insurance Cost Prediction

## Overview
This project predicts insurance costs using machine learning models based on demographic and health-related data. It involves data cleaning, preprocessing, exploratory data analysis (EDA), model training, evaluation, and model comparison.

## Usage

1. Open `Insurance_Cost_Prediction.ipynb` using Google Colab or Jupyter Notebook.
2. Execute each cell to load data, preprocess, train models, and evaluate predictions.
3. Modify parameters or models for experimentation.

## Data

The dataset (`insurance.csv`) contains information including age, sex, BMI, children, smoker status, and region.

**Dataset Details:**
- Number of Rows: 1338
- Number of Columns: 7
- Memory Usage: 0.28 MB.

### Data Cleaning and Preprocessing

- Data cleaning involves handling missing values and removing duplicates from the dataset.
- Categorical variables (sex, smoker, region) are encoded numerically using LabelEncoder.
- Exploratory data analysis (EDA) techniques, including correlation heatmaps and distribution plots, are used to understand data relationships.

### Exploratory Data Analysis (EDA)

- Seaborn is utilized to visualize the distributions of variables like age and BMI.
- Scatter plots analyze relationships between independent variables and charges.

## Models

Three models were evaluated for predicting insurance costs:

1. **Linear Regression**
   - Mean Squared Error: 40431756.87618857
   - Mean Absolute Error: 4427.560035535579
   - R-squared: 0.7404532519935141

2. **SVR (Support Vector Regressor)**
   - Best Parameters: 160484848.02056515
   - Best Score: 8177.211156983577
   - Test Set Score: -0.030212971838076808

3. **Random Forest Regressor**
   - Best Parameters: 160484848.02056515
   - Best Score: 8177.211156983577
   - Test Set Score: -0.030212971838076808

### Model Training and Evaluation

- The dataset is split into training and testing sets using `train_test_split` from Scikit-Learn.
- Numerical features are standardized with `StandardScaler` for optimal model performance.
- Hyperparameter tuning is performed using `GridSearchCV` to find the best parameters for each model.

## Contributing

Contributions are welcome! Please fork the repository and submit pull requests with improvements or additional features.



