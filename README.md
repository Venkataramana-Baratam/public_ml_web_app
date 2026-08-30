A machine learning web application built with **Python** and **Streamlit** that provides prediction interfaces for three diseases:

- Diabetes
- Heart Disease
- Parkinson's Disease

The application uses pre-trained machine learning models saved as `.sav` files and provides an interactive sidebar to switch between the prediction modules.

## 🌐 Live Demo

[Multiple Disease Prediction System](https://publicmlwebapp-mngmcq87psasr3dixe567b.streamlit.app/)

## ✨ Features

- Simple and interactive Streamlit interface
- Sidebar navigation between three prediction modules
- Diabetes prediction
- Heart disease prediction
- Parkinson's disease prediction
- Uses pre-trained machine learning models
- Displays the prediction result directly in the application

## 🧠 Prediction Modules

### 1. Diabetes Prediction

The Diabetes Prediction page accepts the following inputs:

- Number of Pregnancies
- Glucose Level
- Blood Pressure
- Skin Thickness
- Insulin Level
- BMI
- Diabetes Pedigree Function
- Age

The inputs are passed to the trained `diabetes_model.sav` model to generate the prediction.

### 2. Heart Disease Prediction

The Heart Disease Prediction page accepts 13 inputs:

- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Serum Cholesterol
- Fasting Blood Sugar
- Resting Electrocardiographic Results
- Maximum Heart Rate Achieved
- Exercise Induced Angina
- ST Depression
- Slope of Peak Exercise ST Segment
- Major Vessels
- Thal

The inputs are passed to the trained `heart_disease_model.sav` model.

### 3. Parkinson's Disease Prediction

The Parkinson's Prediction page accepts voice-related features including:

- MDVP:Fo(Hz)
- MDVP:Fhi(Hz)
- MDVP:Flo(Hz)
- MDVP:Jitter(%)
- MDVP:Jitter(Abs)
- MDVP:RAP
- MDVP:PPQ
- Jitter:DDP
- MDVP:Shimmer
- MDVP:Shimmer(dB)
- Shimmer:APQ3
- Shimmer:APQ5
- MDVP:APQ
- Shimmer:DDA
- NHR
- HNR
- RPDE
- DFA
- spread1
- spread2
- D2
- PPE

The inputs are passed to the trained `parkinsons_model.sav` model.

## 🛠️ Technologies Used

- **Python**
- **Streamlit** — web application framework
- **NumPy** — numerical computing
- **Pandas** — data handling
- **Scikit-learn** — machine learning
- **Streamlit Option Menu** — sidebar navigation
- **Pickle** — loading the saved machine learning models

## 📂 Project Structure

```text
public_ml_web_app/
│
├── mdps_public.py
├── requirements.txt
├── diabetes_model.sav
├── heart_disease_model.sav
└── parkinsons_model.sav
