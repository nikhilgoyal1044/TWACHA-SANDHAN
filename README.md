# TWACHA-SANDHAN
Dermatological Manifestation Detection Using Machine Learning (SIH)

An AI-powered skin disease detection system developed as part of the Smart BU Internal Hackathon for the Smart India Hackathon (SIH) 2023. The project addresses Problem Statement 1344, aiming to provide a preliminary diagnosis of dermatological diseases using deep learning and computer vision, especially in areas with limited healthcare infrastructure.

📌 Problem Statement

Many rural and remote regions face challenges such as:

Limited access to dermatologists and screening facilities.
Poor internet connectivity affecting online diagnostic tools.
Delayed diagnosis due to lack of medical infrastructure.

This project provides an AI-assisted preliminary screening solution that works efficiently even with intermittent internet connectivity.

🚀 Features
AI-based skin disease prediction from uploaded images.
FastAPI backend for real-time inference.
Deep Learning model built using TensorFlow/Keras.
Image preprocessing with OpenCV and NumPy.
REST APIs for prediction and chat support.
Deployable backend and static frontend.
Designed for low-connectivity environments.
🛠️ Tech Stack
Frontend
HTML5
CSS3
JavaScript
Backend
FastAPI
Python 3.11
Uvicorn
Machine Learning
TensorFlow
Keras
OpenCV
NumPy
Scikit-learn
Deployment
Render
Railway
Azure Web Apps
Fly.io
PythonAnywhere
Vercel (Frontend)
📂 Project Structure
Dermatological-Manifestation-SIH/
│
├── backend1/
│   ├── app.py
│   ├── requirements.txt
│   ├── runtime.txt
│   ├── output/
│   │   ├── best_model.h5
│   │   └── label_map.json
│   └── Procfile (optional)
│
├── assets/
│   └── js/
│       └── detect.js
│
├── render.yaml
├── README.md
└── ...
⚙️ Installation

Clone the repository:

git clone https://github.com/your-username/Dermatological-Manifestation-SIH.git
cd Dermatological-Manifestation-SIH

Create a virtual environment:

cd backend1

python -m venv tf_env

# Windows
tf_env\Scripts\activate

# Linux/Mac
source tf_env/bin/activate

Install dependencies:

pip install -r requirements.txt
▶️ Run the Backend
cd backend1

uvicorn app:app --reload

The API will start on:

http://127.0.0.1:8000

Swagger Documentation:

http://127.0.0.1:8000/docs
📦 Model Files

The following files are required but are not included in the repository because of their size.

backend1/output/
├── best_model.h5
└── label_map.json

You can store them using:

Git LFS
Google Drive
Release Assets
Cloud Storage
🌐 Deployment
Backend (Render)

Build Command

python -m pip install --upgrade pip && pip install -r requirements.txt

Start Command

uvicorn app:app --host 0.0.0.0 --port $PORT

Python Version:

Python 3.11
🎨 Frontend Configuration

Before loading detect.js, configure the backend URL:

<script>
window.BACKEND_URL = "https://your-backend-url.onrender.com";
</script>

Then deploy the frontend using:

Vercel
Netlify
GitHub Pages
📡 API Endpoints
Method	Endpoint	Description
POST	/predict	Predict skin disease
POST	/chat	Chat support endpoint
GET	/docs	Swagger API documentation
🎯 Project Objectives
Assist in preliminary skin disease diagnosis.
Improve accessibility to healthcare in rural areas.
Enable offline-friendly AI inference.
Support future model updates through remote deployment.
Reduce diagnosis time using AI.
👨‍💻 My Contribution
Developed the FastAPI backend.
Integrated the TensorFlow deep learning model.
Implemented image preprocessing and prediction pipeline.
Created REST APIs for disease prediction.
Configured deployment on cloud platforms.
Tested APIs and improved backend performance.
📈 Future Improvements
Mobile application integration.
Multi-language support.
Improved model accuracy with larger datasets.
MLOps pipeline for automatic model updates.
Cloud monitoring and analytics dashboard.
