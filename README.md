Flight Fare Prediction
This project predicts flight fares based on various factors such as departure and arrival times, airline, source, destination, total stops, and flight duration. The prediction is powered by a machine learning model built using Random Forest, which is integrated into a Flask web application to allow users to input flight details and receive fare predictions.

Features
Machine Learning Model: A pre-trained Random Forest model (flight_predict_rf.pkl) predicts flight fares.
Web Application: A Flask-based web app with an intuitive form where users input flight details such as date of journey, airline, number of stops, etc.
Real-time Prediction: Once the user submits the flight information, the model predicts the fare and displays it on the web page.

Project Structure
.
├── app.py                 # Flask application code
├── flight_predict_rf.pkl   # Pre-trained Random Forest model
├── templates
│   └── home.html          # Front-end HTML for input and output
├── static
│   └── style.css          # CSS for styling the web page (optional)
└── README.md              # Project documentation

Installation
To run the project locally, follow these steps:

Prerequisites
Python 3.x
Flask
Pandas
Scikit-learn
Pickle

Input Format
Date of Journey: The date and time of departure (format: YYYY-MM-DDTHH:MM).
Arrival Time: The expected arrival time of the flight.
Total Stops: Number of stops the flight makes (0 for direct flights).
Airline: Select the airline from the dropdown options.
Source: The city of departure.
Destination: The city of arrival.
Example
Input: Departure from Delhi on 2024-09-20T18:30, arrival at 21:30, airline: IndiGo, no stops.
Output: Your Flight price is Rs. 4000

Future Improvements
Include additional features like flight class and demand-based pricing.
Improve the UI with a responsive design.
Add error handling for invalid inputs.
