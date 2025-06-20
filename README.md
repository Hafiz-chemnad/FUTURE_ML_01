# AI-Powered Sales Forecasting Dashboard - Future Interns ML Internship Task 1

## Project Overview
This repository contains the solution for Task 1 of the Future Interns Machine Learning Internship. The objective was to build an AI-powered dashboard that predicts future sales trends using historical retail sales data. The project showcases end-to-end time series forecasting, from data preprocessing and exploratory data analysis to model building and visualization of predictions.

## Objective
The primary goal of this task was to develop a robust sales forecasting model capable of identifying trends and seasonality, and to present these insights through clear, comprehensive visualizations. This dashboard aims to provide actionable intelligence for business planning and decision-making.

## Dataset
The project utilized a fictional retail sales dataset, providing transactional records including date, customer details, product categories, quantities, prices, and total sales amounts. This dataset was instrumental in analyzing historical sales patterns and generating future predictions.

* **Source:** [Link to Kaggle Dataset](https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset?resource=download)

## Methodology
The project followed a structured approach to build the sales forecasting dashboard:

### Data Loading & Initial Inspection
Loaded the raw `retail_sales_dataset.csv` and performed initial checks on its structure and data types.

### Data Preprocessing
Cleaned the data, converted the 'Date' column to datetime format, handled any potential missing values in sales, and aggregated individual transactions into a daily time series of total sales. This prepared the data for time series modeling, specifically formatted for the Prophet library (columns `ds` for date and `y` for sales value).

### Exploratory Data Analysis (EDA)
Conducted a thorough analysis of historical sales data. Visualizations were generated to identify overall trends (e.g., growth, stability), yearly seasonality (e.g., holiday impacts), and weekly seasonality (e.g., weekend sales patterns).

### Forecasting Model Selection & Training
Utilized Facebook Prophet, a powerful and robust time series forecasting library known for handling seasonality, holidays, and trend changes effectively. The model was trained on the processed historical daily sales data.

### Prediction & Visualization
Generated future sales predictions for the next 30 days. These predictions, along with their confidence intervals, were visualized alongside the historical data. Separate plots were also generated to show the decomposed components of the forecast (trend, yearly seasonality, weekly seasonality), forming the interactive "dashboard" within the Jupyter Notebook.

## Deliverables
The core deliverable for this task is the Google Colab / Jupyter Notebook (`FUTURE_ML_01.ipynb`) which serves as the interactive dashboard. It comprehensively includes:
* All Python code for data loading, preprocessing, EDA, model training, and visualization.
* Clear and annotated plots showing historical sales trends, monthly/weekly seasonality, and the main sales forecast with confidence intervals.
* Visualizations of the individual forecast components (trend, yearly, and weekly seasonality).
* Detailed Markdown cells providing explanations for each step, observations from EDA, model choices, and interpretations of the forecast.

## How to Run
To run this notebook and explore the AI-powered sales forecasting dashboard:

### Clone this repository:
```bash
git clone [https://github.com/YourGitHubUsername/FUTURE_ML_01.git](https://github.com/YourGitHubUsername/FUTURE_ML_01.git)
cd FUTURE_ML_01
