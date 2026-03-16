📊 Customer Churn ML Project v5

Advanced Machine Learning pipeline for predicting customer churn using modern MLOps practices.

This project demonstrates how to build a production-ready ML system including training pipeline, experiment tracking, API deployment, and interactive dashboards.

🚀 Features

⚙️ Machine Learning Pipeline using XGBoost

📈 Experiment Tracking with MLflow

🔌 Prediction API built with FastAPI

📊 Interactive Dashboard using Streamlit

🐳 Dockerized Deployment for portability

🧠 End-to-end MLOps workflow

🧱 Project Structure
customer-churn-ml/
│
├── api/
│   └── app.py              # FastAPI prediction service
│
├── src/
│   └── train_model.py      # Training pipeline
│
├── dashboard/
│   └── app.py              # Streamlit dashboard
│
├── models/                 # Saved trained models
│
├── data/                   # Dataset storage
│
├── docker/
│   └── Dockerfile
│
├── requirements.txt
│
└── README.md
⚡ Installation

Clone the repository:

git clone https://github.com/yourusername/customer-churn-ml.git
cd customer-churn-ml

Create a virtual environment:

python -m venv venv

Activate the environment:

Windows

venv\Scripts\activate

Linux / Mac

source venv/bin/activate

Install dependencies:

pip install -r requirements.txt
🧠 Train the Model

Run the training pipeline:

python src/train_model.py

This will:

preprocess the dataset

train the XGBoost model

track experiments using MLflow

save the trained model

🔌 Run Prediction API

Start the FastAPI service:

uvicorn api.app:app --reload

API will be available at:

http://127.0.0.1:8000

Swagger documentation:

http://127.0.0.1:8000/docs
📊 Run Dashboard

Launch the Streamlit dashboard:

streamlit run dashboard/app.py

This dashboard allows you to:

visualize churn predictions

explore customer features

interact with the model

🐳 Docker Deployment

Build the container:

docker build -t churn-ml .

Run the container:

docker run -p 8000:8000 churn-ml
📦 Tech Stack

Python

XGBoost

Scikit-learn

MLflow

FastAPI

Streamlit

Docker

📈 Future Improvements

Model monitoring

CI/CD pipeline

Automated retraining

Feature store integration

Cloud deployment (AWS/GCP)

🤝 Contributing

Contributions are welcome.

Fork the project

Create a feature branch

Commit your changes

Open a Pull Request

📜 License

MIT License
