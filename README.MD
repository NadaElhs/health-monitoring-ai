# Health Monitoring — AI Model
## Overview

Ce projet contient la partie AI d’un système de surveillance de santé.
Il analyse les données de fréquence cardiaque, température corporelle et saturation en oxygène (SpO2) pour :

Classifier l’état de santé du patient
Détecter des anomalies (tachycardie, bradycardie, fièvre)
Prédire des tendances à partir des données historiques

L’AI est exposée via une API Flask indépendante, prête à être appelée par le backend principal ou intégrée dans une architecture microservice.

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
