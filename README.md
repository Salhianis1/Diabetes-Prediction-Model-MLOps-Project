# 🩺 Diabetes Prediction Model – Your First MLOps Project (FastAPI + Docker + K8s)


This project helps you learn **Building and Deploying an ML Model** using a simple and real-world use case: predicting whether a person is diabetic based on health metrics. We’ll go from:

- ✅ Model Training
- ✅ Building the Model locally
- ✅ API Deployment with FastAPI
- ✅ Dockerization
- ✅ Kubernetes Deployment

---
# 📊 Problem Statement

Diabetes is one of the most common chronic diseases worldwide, and early detection plays a key role in preventing severe complications.  
The challenge is to create a system that can **predict whether a person is likely to have diabetes** using simple health indicators.

## 🔑 Input Features
- **Pregnancies** – Number of times the person has been pregnant  
- **Glucose** – Blood sugar level  
- **Blood Pressure** – Blood pressure value  
- **BMI** – Body Mass Index (weight in relation to height)  
- **Age** – Age of the individual  

## 🤖 Machine Learning Approach
We use a **Random Forest Classifier** trained on the well-known **Pima Indians Diabetes Dataset**.  
The model learns patterns that distinguish diabetic from non-diabetic individuals and can then be used to make predictions for new patients.

## 🎯 Goal
The aim of this project is to **provide a practical machine learning solution** that can help in risk assessment and raise awareness about diabetes in an accessible and user-friendly way.

We use a Random Forest Classifier trained on the **Pima Indians Diabetes Dataset**.

---

## 🚀 Quick Start

### 1. Clone the Repo

```bash
git clone https://github.com/Salhianis1/Diabetes-Prediction-Model-MLOps-Project.git
cd Diabetes-Prediction-Model-MLOps-Project
```

### 2. Create Virtual Environment

```
python3 -m venv .mlops
source .mlops/bin/activate
```

### 3. Install Dependencies

```
pip install -r requirements.txt
```

## Train the Model

```
python train.py
```

## Run the API Locally

```
uvicorn main:app --reload
```

### Sample Input for /predict

```
{
  "Pregnancies": 3,
  "Glucose": 90,
  "BloodPressure": 62,
  "BMI": 26,
  "Age": 30
}
```

## Dockerize the API

### Build the Docker Image

```
docker build -t diabetes-prediction-model .
```

### Run the Container

```
docker run -p 8000:8000 diabetes-prediction-model
```

## Deploy to Kubernetes

```
kubectl apply -f diabetes-prediction-model-deployment.yaml
```

🙌 Credits

Created by `SALHI ANIS`

