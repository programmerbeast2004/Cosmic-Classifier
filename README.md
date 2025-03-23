# Cosmic Classifier

📌 Overview

The Cosmic Classifier project is a machine learning model designed by our team to classify planets based on their habitability and resource availability. This project is part of the Galactic Classification Challenge (GCC), where we analyze planetary data to ensure humanity’s survival.

📖 Problem Statement

In the year 2547, Dr. Klaus Reinhardt transmitted planetary classification data before being lost in a black hole. However, due to gravitational interference, parts of the data were corrupted or lost. Our mission was to process this dataset and classify planets into ten predefined categories.

The dataset consists of 10 planetary attributes, and our goal was to develop a robust machine learning model to classify planets based on their survival potential.

🔧 Data Preprocessing

As a team, we focused on ensuring the dataset was clean and optimized for training. The steps we took included:

- Handling missing values: Some data points were lost during transmission, so we filtered them out.
- Scaling features: We used StandardScaler to normalize numerical attributes.
- Feature selection: We identified and retained the most significant planetary attributes for better classification.
- Noise removal: We cleaned the dataset from corrupted entries and outliers to enhance model performance.

🚀 Model Training

We experimented with 10 different machine learning models to find the most accurate classifier. The models we tested included:

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. K-Nearest Neighbors (KNN)
5. Support Vector Classifier (SVC)
6. XGBoost
7. Gradient Boosting
8. Neural Networks
9. Naïve Bayes
10. Extra Trees Classifier

🎯 Best Model Selection

After rigorous testing, we found that SVC (Support Vector Classifier) emerged as the best-performing model, achieving an accuracy of 92% on the test set. This model was chosen based on its ability to handle noisy data effectively and maintain high classification precision.

📊 Results & Evaluation

**Final Model:** SVC

**Accuracy:** 92%

**Performance Metrics:**

- Precision: High across multiple categories
- Recall: Effectively classified difficult cases
- F1-Score: Balanced across all labels

Our team ensured that the final model was well-tuned and optimized to achieve the best possible results.

Project Structure

ML/
│── Code/
│   ├── app.ipynb                     # Jupyter Notebook for model training & evaluation
│
│── Dataset/
│   ├── cosmictest.csv                 # Test dataset for model predictions
│   ├── thermoracleTest.csv            # Additional test dataset
│   ├── thermoracleTrain.csv           # Training dataset used for model learning
│
│── Model/
│   ├── best_svc_Model.pkl             # Trained SVC model with 92% accuracy
│   ├── num_pipeline.pkl               # Preprocessing pipeline for numerical features
│
│── Predictions/
│   ├── Final_predictions.csv          # CSV file containing final model predictions
