# Diabetes Prediction API 🩺

A Machine Learning-based Diabetes Prediction System built using **Python, Scikit-learn, and FastAPI**. The application uses a trained Support Vector Classifier (SVC) model to predict whether a person is likely to have diabetes based on medical input parameters.

## 🚀 Project Overview

This project demonstrates how a trained Machine Learning model can be deployed as a REST API using FastAPI.

Users can submit health-related parameters through an API request and receive a prediction in JSON format.

## 🛠️ Tech Stack

- **Programming Language:** Python
- **Machine Learning:** Scikit-learn
- **ML Algorithm:** Support Vector Classifier (SVC)
- **Backend Framework:** FastAPI
- **Data Validation:** Pydantic
- **Model Serialization:** Pickle
- **API Testing:** Swagger UI

## 📊 Input Features

The model accepts the following eight input parameters:

1. Pregnancies
2. Glucose
3. Blood Pressure
4. Skin Thickness
5. Insulin
6. BMI
7. Diabetes Pedigree Function
8. Age

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Diabetes-Prediction-API.git
cd Diabetes-Prediction-API
```

### 2. Create and activate a virtual environment

```bash
python -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the FastAPI server

```bash
uvicorn ml_api:app --reload
```

### 5. Access API documentation

Open the following URL in your browser:

```text
http://127.0.0.1:8000/docs
```

## 🔗 API Endpoint

**POST** `/diabetes_prediction`

Example request:

```json
{
  "Pregnancies": 2,
  "Glucose": 120,
  "BloodPressure": 70,
  "skinThickness": 25,
  "Insulin": 80,
  "bmi": 28.5,
  "DiabetesPedigreeFunction": 0.5,
  "Age": 35
}
```

Example response:

```json
"The person is not diabetic"
```

The actual response depends on the model prediction.


## 💡 Key Learnings

- Deploying a trained Machine Learning model using FastAPI.
- Creating REST API endpoints for ML inference.
- Validating incoming data using Pydantic.
- Loading serialized ML models using Pickle.
- Testing REST APIs using Swagger UI.

## ⚠️ Disclaimer

This project is intended for educational and demonstration purposes only. Its predictions are not medical diagnoses and should not be used as a substitute for professional medical advice.

## 👨‍💻 Author

**Advait Kulkarni**

