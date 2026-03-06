# 🐔 Chicken Disease Classification

An end-to-end **Deep Learning & MLOps project** that detects chicken diseases from images using Convolutional Neural Networks (CNN). This project demonstrates data ingestion, model training, evaluation, experiment tracking, and deployment using Flask and Docker.

---

## 📌 Project Overview

Poultry diseases can cause major losses for farmers. This project helps in automatically identifying whether a chicken is healthy or infected using image classification.

The project covers:

* Data Ingestion
* Data Validation
* Data Transformation
* Model Training
* Model Evaluation
* Model Deployment
* CI/CD Integration

---

## 🚀 Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* Flask
* DVC (Data Version Control)
* MLflow (optional for experiment tracking)
* Docker
* GitHub Actions (CI/CD)

---

## 🗂 Project Structure

```
Chicken-Disease-Classification/
│
├── .github/workflows/        # CI/CD pipelines
├── config/                   # Configuration files
├── research/                 # Jupyter notebooks & experiments
├── src/                      # Source code
│   └── cnnClassifier/        # ML pipeline modules
├── templates/                # HTML templates for Flask app
├── app.py                    # Flask application
├── main.py                   # Training pipeline entry point
├── params.yaml               # Model parameters
├── requirements.txt          # Dependencies
├── Dockerfile                # Docker configuration
└── README.md
```

---

## ⚙️ How It Works

### 1️⃣ Data Ingestion

* Download dataset
* Store in artifacts folder
* Track using DVC

### 2️⃣ Data Validation

* Check data format
* Ensure no missing or corrupted files

### 3️⃣ Data Transformation

* Resize images
* Normalize pixel values
* Create train/test splits

### 4️⃣ Model Training

* Build CNN model
* Train on training dataset
* Save trained model

### 5️⃣ Model Evaluation

* Evaluate on test dataset
* Generate accuracy and loss metrics

### 6️⃣ Deployment

* Flask API for predictions
* Docker containerization
* CI/CD for automation

---

## 🛠 Installation Guide

### Step 1: Clone Repository

```
git clone <your-repository-link>
cd Chicken-Disease-Classification
```

### Step 2: Create Virtual Environment

```
conda create -n chicken python=3.8 -y
conda activate chicken
```

### Step 3: Install Dependencies

```
pip install -r requirements.txt
```

### Step 4: Run Training Pipeline

```
python main.py
```

### Step 5: Run Flask App

```
python app.py
```

Open in browser:

```
http://localhost:5000
```

---

## 🐳 Run with Docker

### Build Docker Image

```
docker build -t chicken-app .
```

### Run Container

```
docker run -p 5000:5000 chicken-app
```

---
### ECR Repo URl : 
    save the url:158975163941.dkr.ecr.eu-north-1.amazonaws.com/chicken

## 📊 Model Output

The model predicts:

* Healthy Chicken
* Diseased Chicken

Outputs prediction confidence score along with classification.

---

## 📈 Future Improvements

* Add more disease categories
* Improve accuracy with Transfer Learning
* Deploy on AWS / Azure
* Add user authentication
* Build React frontend

---

## 🤝 Contribution

Contributions are welcome! Feel free to fork this repository and submit a pull request.

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 👨‍💻 Author

Tejesh Yewale 

If you like this project, don’t forget to ⭐ the repository!
