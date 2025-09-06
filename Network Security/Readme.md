# 🚀 Network Security Machine Learning Project

## 📌 Overview

#### This project is an end-to-end machine learning pipeline designed to detect and classify malicious vs. legitimate URLs/web traffic.

#### Unlike simple Jupyter notebooks, this project follows a modular, production-ready architecture similar to real-world industry applications. It demonstrates best practices in:

1) Data ingestion & preprocessing
2) Model training & hyperparameter tuning
3) Experiment tracking (MLflow ready – optional)
4) Model evaluation & saving
5) Deployment-ready architecture (Flask/FastAPI API support)

# 🏗️ Project Architecture

```
Network Security Project
│
├── data/                         # Raw & processed datasets
├── networksecurity/
│   ├── components/               # Data pipeline components
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   ├── model_trainer.py
│   │   └── model_evaluation.py
│   │
│   ├── pipeline/                 # Pipeline orchestration
│   │   └── training_pipeline.py
│   │
│   ├── utils/                    # Utility functions
│   │   └── main_utils.py
│   │
│   ├── exception/                # Custom exception handling
│   └── logger/                   # Centralized logging
│
├── final_model/                  # Saved trained model (.pkl)
├── app.py                        # Flask/FastAPI app for prediction
├── main.py                       # Entry point to run full pipeline
└── README.md                     # Project documentation
```

## ⚙️ Pipeline Stages

#### 1️⃣ Data Ingestion  
Load dataset From MONGO DB   
Train-test split  

#### ️2️⃣ Data Transformation
Handle missing values  
Encoding categorical features  
Feature scaling

#### 3️⃣ Model Training  
Multiple ML models tested  
Hyperparameter tuning  
Selection of best-performing model  

#### 4️⃣ Model Evaluation  
r2_SCORE, Precision, Recall, F1-Score   
Save metrics for monitoring   

#### 5️⃣ Model Saving
Export final model as final_model/model.pkl  
Ready for deployment  

#### 6️⃣ Deployment 
Flask/FastAPI app exposes /predict endpoint  
Accepts Input JSON and returns prediction  


## 🛠️ Tech Stack

#### Programming Language: Python 3.11+
#### Database: MONGODB
#### Libraries:
scikit-learn – ML models & preprocessing  
pandas, numpy – Data handling  
matplotlib, seaborn – Visualization  
pickle – Model persistence  
flask / fastapi – Deployment    

## 📊 Results

Multiple models compared (Random Forest, AdaBoost, etc.)  
Final best model stored as model.pkl  
Evaluation metrics logged for future improvement  

## 📈 Future Improvements

Integrate real-time threat detection API  
Deploy using  AWS  
Implement monitoring & model retraining pipeline  

## 👨‍💻 Author

### Vansh Dhall
📌 Aspiring Data Scientist | Machine Learning Enthusiast | Industry-focused Learner