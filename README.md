## 📊 Machine Learning Projects

This repository contains end-to-end Machine Learning projects implemented using a modular, configuration-driven pipeline architecture. The projects demonstrate the complete machine learning lifecycle, from data ingestion to model evaluation, following industry-standard MLOps best practices.

The repository integrates MLflow for experiment tracking and DagsHub for remote experiment logging and collaboration, enabling reproducibility and systematic comparison of models.

## 🚀 Key Features
- End-to-end Machine Learning pipelines
- Modular and reusable project structure
- Configuration-driven workflows using YAML
- Data ingestion, validation, and transformation
- Model training and evaluation
- Experiment tracking using MLflow
- Remote MLflow tracking with DagsHub
- Emphasis on reproducibility and clean architecture

## 🗂️ Typical Project Structure
```
Projects/
├── config/
│   └── config.yaml
│
├── src/
│   └── mlProject/
│       ├── components/
│       │   ├── data_ingestion.py
│       │   ├── data_validation.py
│       │   ├── data_transformation.py
│       │   ├── model_trainer.py
│       │   └── model_evaluation.py
│       │
│       ├── pipeline/
│       │   ├── stage_01_data_ingestion.py
│       │   ├── stage_02_data_validation.py
│       │   ├── stage_03_data_transformation.py
│       │   ├── stage_04_model_trainer.py
│       │   └── stage_05_model_evaluation.py
│       │
│       ├── config/
│       ├── entity/
│       ├── utils/
│       └── logger/
│
├── artifacts/
│
├── main.py
├── requirements.txt
└── README.md
```

## 🛠️ How to Run a Project
### Step 1: Clone the Repository
```
git clone https://github.com/vyash0048-bit/Projects.git
cd Projects
```
### Step 2: Create and Activate Conda Environment
```
conda create -n mlproj python=3.8 -y
conda activate mlproj
```
### Step 3: Install Dependencies
```
pip install -r requirements.txt
```
### Step 4: Run the ML Pipeline
```
python main.py
```
This executes the complete ML workflow:
- Data Ingestion
- Data Validation
- Data Transformation
- Model Training
- Model Evaluation
- MLflow Experiment Logging

### 📊 MLflow Experiment Tracking
▶ Local MLflow UI (Optional)

mlflow ui

Open in browser:http://127.0.0.1:5000

Note: Local MLflow UI displays only local runs.
### 🌐 DagsHub Integration (Remote Tracking)

Experiments can be logged remotely to DagsHub.

Set Environment Variables (Windows)
```
setx MLFLOW_TRACKING_URI "https://dagshub.com/vyash0048/Projects.mlflow"
setx MLFLOW_TRACKING_USERNAME "vyash0048"
setx MLFLOW_TRACKING_PASSWORD "<YOUR_DAGSHUB_TOKEN>"
```

Restart the terminal after setting environment variables.

View Experiments on DagsHub
https://dagshub.com/vyash0048/Projects
→ Experiments → MLflow
DagsHub, following MLOps best practices.
Review the repo like a hiring manager

Just tell me 👍
