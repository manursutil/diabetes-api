# Diabetes Prediction API

A simple API for a diabetes prediction model using the FastAPI library.

## Model Overview

The machine learning model used here was trained to predict diabetes based on the following features:

- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age

The model is stored in `diabetes_model.sav` and loaded at runtime.

## Project Structure

```
.
├── api.py                # Main API server using FastAPI
├── api_test.py           # Simple test script to validate the API
├── diabetes_model.ipynb  # Jupyter Notebook for training the model
├── diabetes_model.sav    # Serialized machine learning model
├── requirements.txt      # List of dependencies

```

## Response format

```
{
    "prediction": 0
}
```

Where 0 means not diabetic, and 1 means likely diabetic.