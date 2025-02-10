# Forest Fire Weather Index Prediction

## Overview

This repository contains a machine learning project aimed at predicting the forest fire weather index (FWI) using regression models. The project leverages RidgeCV and ElasticNetCV algorithms to provide accurate predictions based on input features related to weather conditions.

## Features

- **Web App**: An interactive web application built with Flask that allows users to input weather conditions and receive a prediction of the forest fire weather index.
- **Regression Models**: Implementation of RidgeCV and ElasticNetCV regression models to ensure robust and accurate predictions.
- **Data Processing**: Comprehensive data processing pipeline to clean and prepare input data for modeling.

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/KrishBhimani/Forest-Fire-Prediction.git
    ```

2. **Create and activate a virtual environment:**
    ```bash
    python3 -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the Flask app:**
    ```bash
    python application.py
    ```

5. **Open the web app:**
    Open your browser and navigate to `http://127.0.0.1:5000/predictdata` to access the web app.

## Usage

1. Open the web app in your browser using the URL provided by running the `python application.py` command.
2. Input the relevant weather features such as temperature, humidity, wind speed, etc.
3. Click on the "Predict" button to get the forest fire weather index prediction.

## Data

The dataset used for this project includes various weather-related features that influence forest fire occurrences. The main features include:
1. Date : (DD/MM/YYYY) Day, month ('june' to 'september'), year (2012)
Weather data observations
2. Temp : temperature noon (temperature max) in Celsius degrees: 22 to 42
3. RH : Relative Humidity in %: 21 to 90
4. Ws :Wind speed in km/h: 6 to 29
5. Rain: total day in mm: 0 to 16.8
FWI Components
6. Fine Fuel Moisture Code (FFMC) index from the FWI system: 28.6 to 92.5
7. Duff Moisture Code (DMC) index from the FWI system: 1.1 to 65.9
8. Drought Code (DC) index from the FWI system: 7 to 220.4
9. Initial Spread Index (ISI) index from the FWI system: 0 to 18.5
10. Buildup Index (BUI) index from the FWI system: 1.1 to 68
11. Fire Weather Index (FWI) Index: 0 to 31.1
12. Classes: two classes, namely Fire and not Fire

## Models

### RidgeCV
RidgeCV is a regression model that includes a regularization parameter to prevent overfitting and improve the model's generalizability.

### ElasticNetCV
ElasticNetCV is a regression model that combines both L1 and L2 regularization, balancing between Ridge and Lasso regression to enhance model performance.

## Results

The models have been evaluated using standard performance metrics, demonstrating a high level of accuracy(upto 98%) in predicting the forest fire weather index. These predictions can be instrumental in forest fire risk management and resource allocation.


## Contact

For any questions or suggestions, feel free to open an issue or contact me at [erkrishbhimani@gmail.com](mailto:erkrishbhimani@gmail.com).

