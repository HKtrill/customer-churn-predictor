# Customer Churn Predictor

A full-stack machine learning application that predicts customer churn and provides interactive visual analytics.  
Built with **FastAPI**, **React (TypeScript)**, **Scikit-learn**, **PyTorch**, **PostgreSQL**, **Docker**, and **AWS**.

---

## 📌 Overview

This project enables businesses to identify customers likely to churn using classical and deep learning models.  
Users upload customer datasets (CSV/XLSX), which are preprocessed to handle missing data and categorical features.  
The backend serves predictions through a FastAPI RESTful API using Logistic Regression and Neural Networks.  
Results are visualized with an interactive React frontend featuring charts and dashboards.

---

## 🚀 Features

- Upload and preprocess customer datasets (CSV/XLSX).  
- Predict churn with Logistic Regression, XGBoost, or Neural Networks (PyTorch).  
- Interactive charts and dashboards with React and Chart.js.  
- Store datasets, predictions, and logs in PostgreSQL.  
- Containerized with Docker for easy deployment.  
- Designed for scalable AWS deployment (Elastic Beanstalk, ECS, or EKS).  
- Optional user authentication with OAuth2 and JWT tokens.

---

## 🛠 Tech Stack

**Backend:**  
- Python 3  
- FastAPI  
- Scikit-learn, XGBoost  
- PyTorch (Deep Learning)  
- Pandas, NumPy  
- SQLAlchemy, Alembic  
- Joblib for model persistence

**Frontend:**  
- React with TypeScript  
- Chart.js  
- Axios

**Database:**  
- PostgreSQL

**Deployment:**  
- Docker  
- AWS (Elastic Beanstalk, ECS, or EKS)

---

## 📊 Dataset

**Source:** [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) (Open-Source)  
Contains 7,043 customer records with demographics, account info, and services, labeled by churn status.

---

## 🗂 Project Roadmap

### ✅ Phase 1: Planning  
- Define scope, dataset, and tech stack.

### ⏳ Phase 2: Model Development (Day 2–3)  
- Data loading and preprocessing in Jupyter.  
- Train Logistic Regression baseline and PyTorch neural network.  
- Evaluate models and save best performing one.

### ⏳ Phase 3: Backend API (Day 4)  
- FastAPI endpoints for file upload, prediction, and analytics.  
- Input validation and error handling.

### ⏳ Phase 4: Frontend (Day 5–6)  
- React components for file upload, results display, and charts.

### ⏳ Phase 5: Database Integration (Day 7)  
- Store files, prediction results, and logs in PostgreSQL.

### ⏳ Phase 6: Testing & Deployment (Day 8–9)  
- Unit and integration testing.  
- Docker containerization.  
- AWS deployment.

---

## 📁 Project Structure (Initial)

customer-churn-predictor/
│
├── backend/
│ ├── app/
│ │ ├── main.py
│ │ ├── api/
│ │ │ ├── routes/
│ │ │ │ ├── upload.py
│ │ │ │ ├── predict.py
│ │ │ │ └── analytics.py
│ │ ├── core/
│ │ ├── models/
│ │ ├── preprocessing/
│ │ ├── tests/
│ │ └── requirements.txt
│ └── Dockerfile
│
├── frontend/
│ ├── src/
│ │ ├── components/
│ │ │ ├── FileUpload.tsx
│ │ │ ├── PredictionTable.tsx
│ │ │ └── Charts.tsx
│ │ ├── pages/
│ │ ├── services/
│ │ └── App.tsx
│ ├── public/
│ ├── package.json
│ └── Dockerfile
│
├── data/
│ ├── raw/
│ ├── processed/
│ └── README.md
│
├── notebooks/
│ └── model_dev.ipynb
│
├── README.md
├── docker-compose.yml
└── .gitignore

---

## 📦 Installation & Setup

*(To be updated during development)*

```bash
git clone https://github.com/yourusername/customer-churn-predictor.git
cd customer-churn-predictor

# Backend
cd backend
pip install -r requirements.txt
uvicorn app.main:app --reload

# Frontend
cd ../frontend
npm install
npm start


