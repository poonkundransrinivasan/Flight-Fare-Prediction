# Flight Fare Prediction

This is a Flask web application that predicts flight fares based on various input parameters such as date of journey, airline, source, destination, number of stops, and travel duration. The prediction is done using a model that was trained by Random Forest regressor. (`flight_predict_rf.pkl`).

Learn how the model was trained: https://github.com/poonkundransrinivasan/Flight-Fare-Prediction-Model-Creation

## Table of Contents
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [How to Run the Application](#how-to-run-the-application)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Model Description](#model-description)

## Project Structure

- **templates/home.html**: Front-end HTML template for user interaction.
- **static/styles.css**: CSS file for styling the user interface (if any styling is applied).
- **flight_predict_rf.pkl**: The trained machine learning model stored using `pickle` for making flight fare predictions.
- **app.py**: Main Python script that contains the Flask web server and the logic for handling user input and generating predictions.
- **README.md**: Documentation of the project, including usage instructions, technologies used, and project structure.

## Prerequisites

- Python 3.x
- Flask
- Pandas
- Scikit-learn
- Pickle

Make sure you have the necessary libraries installed by running:

```bash
pip install Flask pandas scikit-learn
```

## Installation
  - Clone the repository:
```bash
git clone https://github.com/poonkundransrinivasan/flight-fare-prediction.git
```
  - Navigate to the project directory:
```bash
cd flight-fare-prediction
```

## How to Run the Application
  - Make sure your flight_predict_rf.pkl model is in the root folder.
  - Run the Flask app:
```bash
python app.py
```
  - Open your browser and navigate to:
    [http://127.0.0.1:5000/](http://127.0.0.1:5000/
    ]

## Usage
1. Enter the date and time of your journey and arrival.
2. Select the number of stops, airline, source, and destination from the dropdown lists.
3. Click the **Predict** button to see the predicted flight fare.

## Technologies Used
- **Flask**: Web framework to run the web application.
- **Scikit-learn**: Machine learning library used for training the Random Forest model.
- **Pandas**: Used for data manipulation and handling datetime operations.
- **Pickle**: To load the trained model for prediction.

## Model Description
The Random Forest model is trained using flight fare data, and the features used for prediction include:
- Date of journey (day and month)
- Departure and arrival time
- Duration of the flight
- Number of stops
- Airline
- Source and destination cities

The model predicts the price of a flight based on these input features.

