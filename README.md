# Credit-Risk-Modelling-Using-machine-Learning
This repository provides a comprehensive solution for credit risk modeling using machine learning techniques. The project analyzes credit-related datasets, performs data preprocessing, applies statistical tests, and trains various machine learning models to predict credit approval probabilities. The deployment is implemented via a Flask-based web application.

Table of Contents
Overview
Features
Technologies Used
Datasets
Project Structure
Installation
Usage
Results
Future Enhancements
Overview
Credit risk modeling is vital for financial institutions to assess borrowers' creditworthiness. This project uses a combination of Random Forest, XGBoost, and Decision Tree models, along with hyperparameter tuning, to predict credit risk categories. The model is deployed using Flask for an interactive interface.

Features
Data Preprocessing

Null value handling
Categorical and numerical feature encoding
Statistical tests (Chi-Square, ANOVA, VIF)
Feature scaling
Machine Learning Models

Random Forest
XGBoost
Decision Tree
Hyperparameter tuning
Deployment

Flask-based web app
User input form for real-time predictions
Evaluation

Accuracy
Precision, Recall, and F1 Score for multi-class outputs
Technologies Used
Programming Language: Python
Libraries: Pandas, NumPy, Scikit-learn, XGBoost, Flask, Matplotlib
Deployment: Flask
Visualization: Matplotlib
Model Saving: Pickle
Datasets
Two datasets (case_study1.xlsx and case_study2.xlsx) were used. These contain information about customer demographics, credit history, and transaction behavior.

Project Structure
php
Copy code
Credit-Risk-Modelling
│
├── mains.py               # Main script for data processing and modeling
├── deploy.py              # Flask application script
├── templates/
│   └── index.html         # HTML template for the web app
├── static/                # Static files for the web app (CSS, JS, etc.)
├── eps_v1.sav             # Pickle file for the trained model
├── README.md              # Project documentation
└── requirements.txt       # Required Python libraries
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/Credit-Risk-Modelling.git
cd Credit-Risk-Modelling
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Ensure you have the datasets in the specified paths.

Place the model (eps_v1.sav) in the root directory.

Usage
Running the Model
Open a terminal in the project directory.

Run the Flask app:

bash
Copy code
python deploy.py
Open a browser and go to http://127.0.0.1:5000/.

Enter input values for features like ROCE (%), CASA (%), etc., and get the prediction.

Training the Model
To train the model from scratch:

Modify the dataset paths in mains.py.
Run mains.py to generate a trained model and save it as eps_v1.sav.
Results
Random Forest: Accuracy: ~85%
XGBoost: Accuracy: ~88% (Best model)
Detailed performance metrics are printed for each class in the terminal.
Future Enhancements
Add more robust preprocessing techniques.
Include deep learning models for enhanced predictions.
Improve the user interface of the Flask app.
