# Automotive Fuel Efficiency Analysis & Prediction

**Author:** Pratik Pawar  
**Project type:** Exploratory Data Analysis (EDA) and Predictive Analytics  
**Domain:** Automotive

## Project Overview

This project explores the factors associated with vehicle fuel efficiency, measured in miles per gallon (MPG), using the historical Auto MPG dataset. It combines data cleaning, exploratory data analysis, group-level comparisons and a baseline Linear Regression model.

The objective is to turn raw vehicle data into understandable findings and evaluate how well selected vehicle specifications can estimate MPG.

> **Dataset context:** The Auto MPG dataset contains historical vehicle observations, primarily from the 1970s and early 1980s. The findings describe this sample and should not be generalized to modern vehicles.

## Business Questions

1. How is fuel efficiency distributed across the vehicles in the dataset?
2. How are vehicle weight, horsepower, displacement and cylinders associated with MPG?
3. How does average MPG vary by vehicle origin?
4. How accurately can a baseline regression model estimate MPG from vehicle specifications?

## Dataset

- **Dataset:** Auto MPG
- **Target variable:** `mpg`
- **Predictors:** cylinders, displacement, horsepower, weight, acceleration, model year and origin
- **Rows:** 398 observations in the commonly distributed dataset
- **Source:** [UCI Machine Learning Repository – Auto MPG](https://archive.ics.uci.edu/dataset/9/auto+mpg)

The notebook loads the dataset through Seaborn and falls back to the UCI raw data source. An internet connection is required unless a local CSV is provided.

## Tools & Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

1. **Data loading and inspection** – review dataset shape, columns, data types and summary statistics.
2. **Data cleaning** – check missing values and duplicates, standardize fields and prepare the target.
3. **Exploratory data analysis** – examine MPG distribution, numeric correlations, scatterplots and average MPG by origin.
4. **Feature preparation** – separate predictors and target, then create a reproducible 80/20 train/test split.
5. **Model development** – use a Scikit-learn pipeline with median/mode imputation, one-hot encoding and Linear Regression.
6. **Model evaluation** – compare the model with a mean-prediction baseline using MAE, RMSE and R-squared.
7. **Interpretation** – discuss patterns, business relevance and limitations without treating correlation as causation.

## Key Analysis Areas

- MPG distribution and spread
- Relationship between MPG and vehicle weight
- Relationship between MPG and horsepower
- Numeric feature correlation
- Average and median MPG by origin
- Actual-versus-predicted values and residual analysis

<img width="1327" height="351" alt="image" src="https://github.com/user-attachments/assets/4765f3be-8688-466d-a28b-4e1adb60b0ed" />

<img width="881" height="592" alt="image" src="https://github.com/user-attachments/assets/ef1a368a-ac7b-485d-a945-1efdb987bd6a" />

<img width="1105" height="419" alt="image" src="https://github.com/user-attachments/assets/ca1368d1-3684-4020-be15-76b8d853e6b5" />

<img width="1099" height="452" alt="image" src="https://github.com/user-attachments/assets/bf5baea7-fb87-471c-8da2-5da5f79ece2d" />

## Model Evaluation

The notebook reports:

| Metric | What it tells us |
|---|---|
| MAE | Average absolute prediction error, in MPG |
| RMSE | Prediction error with larger errors penalized more heavily, in MPG |
| R-squared | Proportion of target variance explained on the test set |

The notebook calculates these values when executed. They are intentionally not hard-coded here because results should be generated from the current notebook run.

## Repository Contents

```text
.
├── Automotive_Fuel_Efficiency_Analysis.ipynb
└── README.md
```

## Findings & Interpretation

Use the generated charts and summary tables in the notebook to identify patterns in this sample. In particular, review how MPG varies with vehicle weight and horsepower and how average MPG differs by origin.

**Important:** These are observational patterns in a historical dataset. Correlation does not prove causation, and the model is a baseline rather than a production-ready vehicle-efficiency estimator.

## Limitations

- The dataset is historical and relatively small.
- Linear Regression may not capture all nonlinear relationships.
- Evaluation depends on the selected train/test split.
- The dataset does not represent today's vehicle technologies or driving conditions.
- Further validation is required before using predictions in real-world decisions.


## Author

**Pratik Pawar**  
Pune, Maharashtra, India

- GitHub: [@pratikpawar6338](https://github.com/pratikpawar6338)
- LinkedIn: [Pratik Pawar](https://www.linkedin.com/in/pratik-pawar-ds/)

---

If you find this project useful, feel free to explore the notebook and share feedback.
