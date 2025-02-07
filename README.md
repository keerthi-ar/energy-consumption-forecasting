# Energy Consumption Forecasting

## Objective:
The goal of this project is to forecast energy consumption patterns to optimize energy usage in smart grids or homes. This will help reduce energy costs and improve the efficiency of energy consumption by predicting future demand.

## Dataset:
This project uses the Household Power Consumption Dataset from the UCI Machine Learning Repository. The dataset contains a detailed record of electrical power consumption for a household, including features such as Global Active Power, Voltage, and more.

- **Dataset URL**: [Household Power Consumption Dataset](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)

## Project Overview:
In this project, we predict future energy consumption based on historical data using ARIMA (AutoRegressive Integrated Moving Average) time-series forecasting. The model is trained on the past energy consumption data, evaluated for performance, and then used to forecast future energy consumption patterns.

The key steps include:
- Data Preprocessing
- Time-Series Forecasting using ARIMA
- Model Evaluation (RMSE and MAE)
- Future Forecasting for Energy Consumption

## Steps Taken:

### 1. **Data Exploration and Preprocessing:**
- Loaded and cleaned the dataset, converting date and time columns into a datetime object.
- Handled missing values by forward filling them.
- Set the datetime column as the index for time-series analysis.

### 2. **Feature Engineering:**
- Extracted additional time-related features like the year, month, day, hour, and weekday to assist with better model performance and analysis.

### 3. **Train-Test Split:**
- Split the data into training and testing datasets. The training dataset consists of 80% of the data, while the remaining 20% is reserved for testing.

### 4. **ARIMA Model Implementation:**
- Applied the ARIMA model for time-series forecasting.
- The ARIMA model was trained using the Global Active Power feature of the dataset.

### 5. **Model Evaluation:**
- Evaluated the model using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) to measure the prediction accuracy.
- The model's performance was visually assessed by plotting forecasted values against actual test values.

### 6. **Future Forecasting:**
- The trained ARIMA model was used to forecast the energy consumption for the next 30 days.
- Results were plotted to visualize future energy consumption patterns.

## Citation:
G. Hebrail and A. Berard. "Individual Household Electric Power Consumption," UCI Machine Learning Repository, 2006. [Online]. Available: https://doi.org/10.24432/C58K54.

## Acknowledgments
Thanks to the UCI Machine Learning Repository for making this dataset publicly available.

## Installation:
To run this project on your local machine, you need to install the following libraries:

```bash
pip install statsmodels pandas matplotlib scikit-learn numpy
```
## Usage:

### Clone the repository:
```bash
git clone https://github.com/your-username/energy-consumption-forecasting.git
```

### Navigate to the project directory:
```bash
cd energy-consumption-forecasting
```

### Install the required libraries:
```bash
pip install -r requirements.txt
```

### Run the Jupyter Notebook:
```bash
jupyter notebook energy-consumption-forecasting.ipynb
```

