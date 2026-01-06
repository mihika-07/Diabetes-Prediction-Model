# Diabetes Prediction Model

## Author
Mihika Goyal  
Second Year Computer Science Engineering Student

---

## Project Overview
This project is a machine learning–based web application designed to predict the risk of diabetes in an individual based on clinical symptoms and demographic information. The system uses a trained Random Forest classifier and provides predictions through a Flask-based web interface.

The objective of this project is to demonstrate the complete machine learning workflow, including data preprocessing, model training, evaluation, serialization, and deployment as a web application.

---

## Problem Statement
Early detection of diabetes is critical for timely medical intervention and prevention of long-term complications. Manual diagnosis based solely on symptoms can be subjective and error-prone. This project aims to automate diabetes risk prediction using supervised machine learning techniques to assist in early screening.

---

## Features
- Predicts diabetes risk based on multiple clinical symptoms and patient attributes
- Trained using a Random Forest classification algorithm
- High prediction accuracy on the Early Diabetes Detection dataset
- Web-based interface built using Flask
- Clean, responsive, and professional user interface
- Color-coded prediction results for better clarity
- Model serialization for efficient deployment

---

## Dataset Information
- Dataset: Early Diabetes Detection Dataset
- Data Type: Structured tabular data
- Features include:
  - Age
  - Gender
  - Polyuria
  - Polydipsia
  - Sudden weight loss
  - Weakness
  - Polyphagia
  - Genital thrush
  - Visual blurring
  - Itching
  - Irritability
  - Delayed healing
  - Partial paresis
  - Muscle stiffness
  - Alopecia
  - Obesity
- Target Variable:
  - Class (Positive: Diabetes Risk, Negative: No Diabetes)

---

## Machine Learning Model
- Algorithm: Random Forest Classifier
- Learning Type: Supervised Learning (Binary Classification)
- Motivation for Selection:
  - Handles categorical and non-linear data efficiently
  - Reduces overfitting using ensemble learning
  - Provides stable and accurate predictions
- Model Training:
  - Data preprocessing and encoding performed prior to training
  - Stratified train-test split used
  - Hyperparameters tuned for optimal performance
- Model Deployment:
  - Trained model serialized using Pickle
  - Loaded directly into Flask application for inference

---

## Project Architecture
- Model training performed offline using a Jupyter Notebook
- Trained model (`model.pkl`) and feature columns (`columns.pkl`) exported
- Flask backend loads the trained model for prediction
- HTML and CSS used for frontend interface
- Predictions processed and displayed in real time

---

## Technologies Used
- Python
- Flask
- Scikit-learn
- Pandas
- NumPy
- HTML
- CSS

---

## Requirements and Dependencies
All required dependencies are listed in the `requirements.txt` file.

```
Flask==3.0.0
pandas==2.2.2
scikit-learn==1.4.2
numpy==1.26.4
```

---

## How to Run the Project Locally

### Step 1: Clone the repository
```
git clone <repository-url>
cd Diabetes-Prediction-Model
```

### Step 2: Create and activate a virtual environment
```
python3 -m venv venv
source venv/bin/activate
```

### Step 3: Install dependencies
```
pip install -r requirements.txt
```

### Step 4: Run the Flask application
```
python3 app.py
```

### Step 5: Open the application
Navigate to the following URL in your web browser:
```
http://127.0.0.1:5000
```

---

## Usage Instructions
- Enter patient details and symptoms in the input form
- Click the Predict button
- The system displays whether diabetes risk is present or not
- Results are visually highlighted for improved clarity

---

## Folder Structure
```
Diabetes-Prediction-Model/
│
├── app.py
├── model.pkl
├── columns.pkl
├── requirements.txt
├── .gitignore
│
├── templates/
│   └── index.html
│
└── static/
    └── style.css
```

---

## Notes
- Virtual environment files are excluded using `.gitignore`
- Model files are included for evaluation and demonstration
- This system is intended for educational and academic purposes only
- It should not be used as a substitute for professional medical diagnosis

---

## Conclusion
This project demonstrates the end-to-end deployment of a machine learning model for healthcare applications. It integrates data preprocessing, model training, evaluation, and web deployment into a unified system, highlighting practical applications of machine learning using industry-standard tools.
