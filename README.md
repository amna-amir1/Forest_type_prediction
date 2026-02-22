🌲 Forest Type Prediction using Machine Learning (XGBoost)

📌 Project Overview

This project focuses on forest type classification using supervised machine learning techniques.
The goal is to predict the type of forest based on multiple environmental and geographical features.

Two machine learning models were trained and evaluated:

Random Forest Classifier

XGBoost Classifier (Final Selected Model)

After performance comparison, XGBoost was selected due to its higher accuracy and better generalization on unseen data.

🎯 Problem Statement

Given a set of numerical features related to forest areas (such as elevation, soil type, slope, etc.), the task is to classify each sample into one of the forest cover types (classes 1 to 7).

This is a multi-class classification problem.

📂 Dataset

The dataset contains multiple numerical features

Target variable: Forest Cover Type (1–7)

No missing values

Data was already clean but required preprocessing for modeling

📎 Dataset Source:

https://www.kaggle.com/competitions/forest-cover-type-prediction/data


🧪 Exploratory Data Analysis (EDA)

The following steps were performed during EDA:

Dataset shape and structure inspection

Feature distribution analysis

Correlation analysis between features

Checking class distribution to understand imbalance

Visualization using histograms

EDA helped in understanding feature importance and data behavior before training models.

⚙️ Data Preprocessing

The following preprocessing steps were applied:

Feature and target separation

Train-test split

Data validation before model training

The preprocessing pipeline ensures consistent input during both training and prediction stages.

🤖 Models Implemented

1️⃣ Random Forest Classifier

Hyperparameter tuning applied

Strong baseline model

Performance:

Training Accuracy: 84%

Testing Accuracy: 82%

Although Random Forest performed well, it was not selected as the final model.

2️⃣ XGBoost Classifier (Final Model)

Hyperparameter tuning applied using optimal parameters

Better handling of complex patterns

Reduced overfitting compared to Random Forest

Performance:

Training Accuracy: 91%

Testing Accuracy: 89%

✅ XGBoost was selected as the final model due to its superior performance.

💾 Model Saving

The trained XGBoost model was saved using serialization so it can be reused without retraining.

Saved files include:

Trained model file

🎨 Gradio Web Interface

A user-friendly Gradio UI was developed for real-time predictions.

🔹 Features of the UI:

Manual user input for all required features

Trained model file used

Instant prediction result

Clean and interactive layout

🔹 Functionality:

User enters feature values

Model predicts forest cover type

Output displays predicted class (1–7)

This UI makes the model easily accessible and deployable.

🚀 How to Run the Project

Clone the repository

Install required libraries

Run the Gradio interface script

Enter feature values in the UI

Get real-time forest type prediction

🛠 Technologies Used

Python

Pandas

NumPy

Scikit-learn

XGBoost

Matplotlib / Seaborn

Gradio

📌 Conclusion

This project demonstrates how machine learning models can be effectively used for multi-class classification problems.
After comparing multiple models, XGBoost proved to be the most reliable and accurate, making it suitable for deployment using an interactive web interface.

🔮 Future Improvements

Add feature importance visualization

Deploy the app on a cloud platform

Improve UI design further

Add model explainability (SHAP / LIME)

👩‍💻 Author

Amna Bibi

Machine Learning Enthusiast
