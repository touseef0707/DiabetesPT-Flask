# Diabetes Prediction Tool - Flask API

This repository contains the backend API for the Diabetes Prediction Tool. It is designed to serve predictions about diabetes based on user input using a RandomForest classifier trained on the diabetes dataset.

## API Endpoint (note: it is currently suspended)

The backend provides a single API endpoint for making predictions:

### `POST /predict_method`

**URL**: `https://diabetespt-flask.onrender.com/predict_method`

**Request Body** (JSON):
```json
{
  "pregnancies": <integer>,
  "glucose": <integer>,
  "bloodPressure": <integer>,
  "skinThickness": <integer>,
  "insulin": <integer>,
  "bmi": <float>,
  "diabetesPedigreeFunction": <float>,
  "age": <integer>
}
```

**Response** (JSON):
```json
{
  "result": "Diabetic" | "Not Diabetic"
}
```

## How to Use

The frontend for this application is deployed at: [https://diabetespt-react-frontend.onrender.com](https://diabetespt-react-frontend.onrender.com)

The frontend repository can be found at: [DiabetesPT-React-FrontEnd](https://github.com/touseef0707/DiabetesPT-React-FrontEnd)

### Steps to Use the Application

1. **Visit the Frontend**: Navigate to [https://diabetespt-react-frontend.onrender.com](https://diabetespt-react-frontend.onrender.com).
2. **Input Data**: Enter the required health metrics such as pregnancies, glucose levels, blood pressure, etc.
3. **Get Prediction**: Click the submit button to send your data to the backend API. The result will display whether the user is "Diabetic" or "Not Diabetic".


This content provides clear instructions and information for users and developers interacting with your backend API and frontend application.
