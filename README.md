# Dermatological Manifestation Detection 

An AI-powered skin disease detection system developed as part of the
**Smart BU Internal Hackathon** for the **Smart India Hackathon (SIH)
2023**. The project addresses **Problem Statement 1344**, aiming to
provide a preliminary diagnosis of dermatological diseases using deep
learning and computer vision, especially in areas with limited
healthcare infrastructure.

## 📌 Problem Statement

Many rural and remote regions face challenges such as:

-   Limited access to dermatologists and screening facilities.
-   Poor internet connectivity affecting online diagnostic tools.
-   Delayed diagnosis due to lack of medical infrastructure.

This project provides an AI-assisted preliminary screening solution that
works efficiently even with intermittent internet connectivity.

## 🚀 Features

-   AI-based skin disease prediction from uploaded images.
-   FastAPI backend for real-time inference.
-   Deep Learning model built using TensorFlow/Keras.
-   Image preprocessing with OpenCV and NumPy.
-   REST APIs for prediction and chat support.
-   Deployable backend and static frontend.
-   Designed for low-connectivity environments.

## 🛠️ Tech Stack

### Frontend

-   HTML5
-   CSS3
-   JavaScript

### Backend

-   FastAPI
-   Python 3.11
-   Uvicorn

### Machine Learning

-   TensorFlow
-   Keras
-   OpenCV
-   NumPy
-   Scikit-learn

### Deployment

-   Render
-   Railway
-   Azure Web Apps
-   Fly.io
-   PythonAnywhere
-   Vercel (Frontend)

## 📂 Project Structure

``` text
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
```

## ⚙️ Installation

``` bash
git clone https://github.com/your-username/Dermatological-Manifestation-SIH.git
cd Dermatological-Manifestation-SIH

cd backend1
python -m venv tf_env

# Windows
tf_env\Scripts\activate

# Linux/Mac
source tf_env/bin/activate

pip install -r requirements.txt
```

## ▶️ Run the Backend

``` bash
cd backend1
uvicorn app:app --reload
```

Open: - http://127.0.0.1:8000 - http://127.0.0.1:8000/docs

## 📦 Model Files

Required files (not included due to size):

``` text
backend1/output/
├── best_model.h5
└── label_map.json
```

Store them using Git LFS, release assets, or external cloud storage.

## 🌐 Deployment

### Backend (Render)

**Build Command**

``` bash
python -m pip install --upgrade pip && pip install -r requirements.txt
```

**Start Command**

``` bash
uvicorn app:app --host 0.0.0.0 --port $PORT
```

Python Version: **3.11**

## 🎨 Frontend Configuration

Before loading `detect.js`:

``` html
<script>
window.BACKEND_URL = "https://your-backend-url.onrender.com";
</script>
```

Deploy the frontend using Vercel, Netlify, or GitHub Pages.

## 📡 API Endpoints

  Method   Endpoint     Description
  -------- ------------ ---------------------------
  POST     `/predict`   Predict skin disease
  POST     `/chat`      Chat endpoint
  GET      `/docs`      Swagger API documentation

## 👨‍💻 My Contribution

-   Developed the FastAPI backend.
-   Integrated the TensorFlow/Keras model.
-   Implemented image preprocessing and prediction APIs.
-   Created REST APIs for frontend integration.
-   Assisted with deployment configuration and testing.

## 🎯 Objectives

-   Preliminary AI-assisted skin disease diagnosis.
-   Improve healthcare accessibility in remote areas.
-   Support offline-friendly deployment.
-   Enable future model updates using MLOps.

## 📄 License

Developed for the **Smart India Hackathon (SIH) 2023** for educational
and research purposes.
