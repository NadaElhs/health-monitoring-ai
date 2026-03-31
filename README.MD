# Health Monitoring — AI Model

## Setup

pip install -r requirements.txt

## Train the model

python train_model.py

## Start the API

python app.py

# API runs on http://localhost:5000

## Main endpoint

POST /predict
Body: { "heart_rate_bpm": 110, "body_temperature_c": 38.9, "spo2_percent": 94.0 }
