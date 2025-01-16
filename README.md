Credit Risk Modelling Using Machine Learning
This repository demonstrates how to build a credit risk modeling solution using machine learning techniques. It includes data preprocessing, statistical analysis, model training, and deployment via a Flask-based web application.
Table of Contents:
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
Credit risk modeling helps financial institutions assess borrowers' creditworthiness. This project uses machine learning models like Random Forest, XGBoost, and Decision Tree to predict credit risk categories. The deployment is done using Flask for real-time interaction.
Features
Data Preprocessing

Handles missing values.
Encodes categorical and numerical features.
Performs statistical tests (Chi-Square, ANOVA, VIF).
Applies feature scaling.
Machine Learning Models

Random Forest
XGBoost
Decision Tree
Hyperparameter tuning for improved accuracy.
Deployment

Flask-based web app for real-time predictions.
Interactive input form for user data.
Evaluation Metrics

Accuracy
Precision, Recall, and F1 Score for multi-class classification.
Technologies Used
Programming Language: Python
Libraries: Pandas, NumPy, Scikit-learn, XGBoost, Flask, Matplotlib
Deployment: Flask Web Framework
Visualization: Matplotlib
Model Saving: Pickle
Datasets
This project uses two datasets:

case_study1.xlsx – Customer demographic data.
case_study2.xlsx – Customer credit and transaction data.
Project Structure
Credit-Risk-Modelling
│
├── mains.py               # Data preprocessing and machine learning models
├── deploy.py              # Flask application for deployment
├── templates/
│   └── index.html         # Frontend template for the web app
├── static/                # Static assets like CSS and JS for the web app
├── eps_v1.sav             # Trained model saved using Pickle
├── README.md              # Project documentation
└── requirements.txt       # Required Python libraries
Installation
Clone the Repository
git clone https://github.com/yourusername/Credit-Risk-Modelling.git
cd Credit-Risk-Modelling
Install Dependencies
pip install -r requirements.txt
Prepare Datasets
Place the datasets (case_study1.xlsx and case_study2.xlsx) in the appropriate directory. Update the file paths in mains.py if needed.

Load the Model
Ensure the trained model (eps_v1.sav) is in the root directory.
Usage
Running the Flask App
Run the Flask application:
python deploy.py
Open your browser and go to:
http://127.0.0.1:5000/
Enter the required feature inputs like ROCE (%), CASA (%), etc., and get predictions.
Training the Model
To retrain the model:

Modify the dataset paths in mains.py.
Execute the script:
python mains.py
Save the generated model as eps_v1.sav.
Results
Random Forest: Accuracy ~85%
XGBoost: Accuracy ~88% (Best-performing model)
Detailed metrics like precision, recall, and F1 scores are displayed in the terminal for each risk category.
Future Enhancements
Add more sophisticated preprocessing techniques.
Introduce deep learning models for better accuracy.
Improve the user interface of the Flask application

Contributions, issues, and suggestions are welcome! Feel free to raise a pull request or log an issue. 😊


