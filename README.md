# Heart Stroke Predictor

## Overview
The Heart Stroke Predictor is a machine learning web application that predicts the risk of heart disease based on various health and demographic factors. Built with Streamlit and scikit-learn, this interactive tool provides instant risk assessments to help identify individuals who may be at higher risk of heart-related conditions.

## About the Project
Heart disease remains one of the leading causes of death globally. Early detection and risk assessment can significantly improve prevention and treatment outcomes. This project uses machine learning to analyze patient data and predict heart disease risk, making it accessible through an easy-to-use web interface.

## Key Features
- **Interactive Web Interface**: User-friendly Streamlit application for easy data input
- **Real-time Predictions**: Instant heart disease risk assessment
- **Multiple Health Indicators**: Analyzes age, blood pressure, cholesterol, ECG results, and more
- **Machine Learning Model**: Logistic regression model trained on comprehensive health data
- **Visual Feedback**: Clear risk indicators with color-coded results

## Technologies Used
- **Python 3.13**
- **Streamlit**: Web application framework
- **scikit-learn**: Machine learning model and data preprocessing
- **pandas**: Data manipulation and analysis
- **joblib**: Model serialization

## Input Parameters
The application accepts the following health metrics:
- Age (18-100 years)
- Sex (Male/Female)
- Chest Pain Type (ATA, NAP, TA, ASY)
- Resting Blood Pressure (mm Hg)
- Cholesterol Level (mg/dL)
- Fasting Blood Sugar (>120 mg/dL)
- Resting ECG Results (Normal, ST, LVH)
- Maximum Heart Rate
- Exercise-Induced Angina (Yes/No)
- Oldpeak (ST Depression)
- ST Slope (Up, Flat, Down)

## How It Works
1. The model uses a Logistic Regression classifier
2. Input features are preprocessed with StandardScaler for numerical values
3. Categorical features are one-hot encoded
4. The trained model predicts risk based on 15 processed features

## Installation & Usage

### Prerequisites
- Python 3.x installed
- pip package manager

### Setup
```bash
# Clone the repository
git clone https://github.com/omgholap11/Heart-Stroke-Predictor.git
cd Heart-Stroke-Predictor

# Install required packages
pip install streamlit scikit-learn pandas joblib

# Run the application
streamlit run app.py
```

The application will open in your default web browser at `http://localhost:8501`

## Model Files
- `logistic_regression_heart.pkl`: Trained machine learning model
- `scaler.pkl`: Fitted StandardScaler for numerical features
- `columns.pkl`: Expected feature columns for model input

## Contributing
Contributions, suggestions, and feedback are welcome! Feel free to open issues or submit pull requests.

## License
This project is open source and available for educational and research purposes.

---
*Note: This tool is intended for educational purposes and should not replace professional medical advice.*
