# 🚗 Used Car Price Prediction App

A machine learning-powered web application built with **Streamlit** that predicts the price of used cars in Malaysia. The app uses a trained **Random Forest** model along with a data preprocessing pipeline that includes scaling and encoding.

## 🔍 Features

- Predict car prices based on user-selected specifications
- Dynamic dropdowns for brand, model, and variant based on sample dataset
- Clean and interactive Streamlit interface
- Built using preprocessed and dimensionally-reduced data for fast prediction

## 📁 Project Structure

- README.md: This file contains important information about the project, how to set it up, and how to run the application.
- app.py: This is the main file for the Streamlit app. It contains the user interface and the logic to interact with the machine learning model, get user input, and make predictions based on the trained model.
- pipeline_xgb.pkl: This file contains the preprocessing pipeline used in the app. It includes steps like one-hot encoding for categorical features, scaling for numeric features, and dimensionality reduction using TruncatedSVD. This is necessary to ensure the input data is processed exactly the same way as the training data.
- model_xgb.pkl: This file stores the trained XGBoost model. The model is used to make predictions based on the processed input features.
- requirements.txt: This file lists all the Python libraries and dependencies that the project requires to run. It is used to set up the environment by installing the necessary packages using the pip install -r requirements.txt command.
- carbrandmodellist.csv : This folder contains any data that the project uses, store a small dataset with brands, models, variants, etc., used to populate dropdown options for the app interface.


## 🧠 Model Info

- **Model**: Random Forest Regressor
- **Preprocessing**:
  - One-Hot Encoding for categorical variables
  - Standard Scaling for numeric variables

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/car-price-prediction-app.git
cd car-price-prediction-app
```

### 2. Install Requirements
```bash
pip install -r requirements.txt
```

### 3. Run the Streamlit App
```bash
streamlit run priceprediction.py
```

## 📝 Notes
The model expects inputs to match the format and features used during training.

Ensure all necessary .pkl files are available in the root directory before running the app.

## 📬 Contact
If you find this useful or have suggestions for improvement, feel free to open an issue or reach out!
