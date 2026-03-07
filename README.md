#  Chicken Disease Classification – MLOps Project

## 📌 Project Overview

This project builds a complete **end‑to‑end MLOps pipeline** to detect chicken diseases from fecal images using a deep learning model. The goal is to help poultry farmers quickly identify diseases and take preventive actions.

The project demonstrates **machine learning + deployment + CI/CD + cloud infrastructure**.

---

# 🚀 Live Application

The project is deployed on AWS EC2 using Docker.

🔗 **Live Demo:**
[http://13.63.53.244:5000](http://13.63.53.244:5000)

---

# 🧠 Problem Statement

Chicken diseases can spread quickly in poultry farms. Manual detection is slow and requires expertise. This system automatically analyzes fecal images and predicts whether the chicken is healthy or infected.

---

# ⚙️ Tech Stack

* **Python**
* **TensorFlow / Keras**
* **Flask (API & Web App)**
* **Docker (Containerization)**
* **AWS EC2 (Deployment)**
* **GitHub Actions (CI/CD)**
* **DVC (Data Version Control)**

---

# 🏗️ Project Architecture

```
User Upload Image
        │
        ▼
Flask Web Application
        │
        ▼
Prediction Pipeline
        │
        ▼
Trained Deep Learning Model
        │
        ▼
Prediction Result
```

---

# 📂 Project Structure

```
Chicken-Disease-Classification-Project
│
├── artifacts/                # Generated outputs (models, logs)
├── config/                   # Configuration files
├── research/                 # Jupyter notebooks
├── src/                      # Source code
│   └── cnnClassifier/
│
├── templates/                # HTML templates
├── app.py                    # Flask web application
├── main.py                   # Training pipeline
├── Dockerfile                # Docker configuration
├── requirements.txt          # Python dependencies
└── README.md
```

---

# 🔬 Machine Learning Pipeline

### 1️⃣ Data Ingestion

Downloads and extracts the chicken disease dataset.

### 2️⃣ Base Model Preparation

Loads a pretrained CNN architecture for transfer learning.

### 3️⃣ Model Training

Trains the network using labeled fecal images.

### 4️⃣ Model Evaluation

Evaluates performance and saves metrics.

### 5️⃣ Prediction Pipeline

Loads the trained model and predicts disease class.

### 6️⃣ Deployment

Deploys the model through a Flask API and Docker container.

---

# 💻 Run the Project Locally

## 1️⃣ Clone Repository

```bash
git clone https://github.com/Tejeshyewale/Chicken-Disease-Classification-Project.git
cd Chicken-Disease-Classification-Project
```

---

## 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

Activate environment

**Windows**

```bash
venv\\Scripts\\activate
```

**Linux / Mac**

```bash
source venv/bin/activate
```

---

## 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4️⃣ Train the Model

```bash
python main.py
```

---

## 5️⃣ Run the Web Application

```bash
python app.py
```

Then open:

```
http://localhost:5000
```

---

# 🐳 Run Using Docker

## Build Docker Image

```bash
docker build -t chicken-disease-app .
```

## Run Container

```bash
docker run -d -p 5000:5000 chicken-disease-app
```

Open:

```
http://localhost:5000
```

---

# ☁️ AWS Deployment

This project is deployed on **AWS EC2** using Docker containers.

Deployment workflow:

1. Push code to GitHub
2. GitHub Actions CI/CD pipeline triggers
3. Docker image builds
4. Image deploys to EC2
5. Flask app runs inside container

---

# 🔁 CI/CD Pipeline

Automated using **GitHub Actions**.

Pipeline stages:

✔ Install dependencies
✔ Build Docker image
✔ Push Docker image
✔ Deploy to AWS EC2

---

# 📊 Model Output

The model predicts two classes:

* **Healthy**
* **Coccidiosis (Chicken Disease)**

Users upload an image and instantly receive a prediction.

---

# 📈 Future Improvements

* Improve model accuracy with larger dataset
* Add real‑time camera prediction
* Build mobile application for farmers
* Add monitoring dashboard

---

# 👨‍💻 Author

**Tejesh Yewale**
Computer Engineering Student

Interests:

* Data Science
* Machine Learning
* MLOps
* Cloud Deployment

---

# ⭐ Support

If you like this project, please give it a ⭐ on GitHub!

Repository:

[https://github.com/Tejeshyewale/Chicken-Disease-Classification-Project](https://github.com/Tejeshyewale/Chicken-Disease-Classification-Project)

---

# 🌐 Run the Project (Live)

👉 **[http://13.63.53.244:5000](http://13.63.53.244:5000)**
