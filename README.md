# Sales Forecasting for Favorita Stores

This repository contains a machine learning project to predict sales for thousands of product families sold at Favorita stores in Ecuador. The goal of this project is to apply time-series forecasting techniques to predict product sales based on historical data.


## Dataset Overview

The project uses the following datasets:

- **train.csv**: The training data containing time-series features such as `store_nbr`, `family`, `onpromotion`, and the target variable `sales`.
- **test.csv**: The test data with the same features as the training data. The task is to predict the sales for the dates in this file.
- **sample_submission.csv**: A sample submission file in the correct format for Kaggle submission.
- **stores.csv**: Metadata about stores, including the city, state, store type, and cluster.
- **oil.csv**: Daily oil price data. This feature could be relevant for sales predictions due to Ecuador's dependence on oil.
- **holidays_events.csv**: Information about holidays and events, including transferred holidays and extra holidays, which could affect sales.

### Problem Context

The project focuses on predicting sales for grocery stores in Ecuador. Retailers must forecast product demand accurately to avoid overstocking and stockouts, both of which can affect profitability and customer satisfaction. By using machine learning techniques, this project aims to improve forecasting accuracy.

### Key Features

- **store_nbr**: Identifier for the store where the product is sold.
- **family**: Product category (e.g., dairy, produce, etc.).
- **sales**: Total sales of a product family at a specific store on a specific date.
- **onpromotion**: Number of units of a product family that were promoted at a store on a given day.
- **date**: The date of the observation.


## Analysis Visualizations
![image](https://github.com/user-attachments/assets/059854c7-239c-439e-9b9f-d227c8ab0120)
![image](https://github.com/user-attachments/assets/a4300771-69d3-4a48-b31f-be90f29462fc)
![image](https://github.com/user-attachments/assets/825738cf-9845-40cc-af15-94bcb686e676)

# And more!


### External Influences

- **Oil Prices**: As an oil-dependent country, fluctuations in oil prices significantly impact the Ecuadorian economy, affecting supermarket sales.
- **Holidays & Events**: Sales data can also be influenced by holidays and national events, which may increase or decrease demand.

### Additional Notes

- The project explores how to handle holidays, promotions, and external factors such as oil prices.
- Special attention should be given to transferred holidays and how they differ from the actual celebration days.
- The 2016 earthquake is a notable event that affected supermarket sales, which could be used as a special feature in modeling.

## Setup and Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/sales-forecasting.git
   cd sales-forecasting
   ```

2. Install the necessary Python packages:
   ```bash
   pip install -r requirements.txt
   ```

## Project Structure

- `data/`: Contains datasets used in this project.
- `notebooks/`: Includes Jupyter notebooks demonstrating data analysis, feature engineering, modeling, and evaluation.
- `models/`: Stores serialized models.

## Technologies Used

- Python
- Pandas
- Matplotlib & Seaborn
- Scikit-learn (RandomForestRegressor, PCA)
- XGBoost

## Contributions

Feel free to contribute by opening issues, submitting pull requests, or providing feedback and suggestions.

