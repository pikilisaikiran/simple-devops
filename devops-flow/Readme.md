# Simple DevOps Project: Flask App with Docker & Kubernetes on Minikube  

This repository contains a **Flask application** that is containerized using **Docker** and deployed on a **Minikube Kubernetes cluster**.  

## 📌 Project Structure  

```
.
├── app
│   ├── app.py           # Flask application
│   ├── Dockerfile       # Dockerfile for building the image
│   ├── Readme.md        # Documentation for the app
│   └── requirements.txt # Python dependencies
├── k8s-deployment
│   └── flink-app.yaml   # Kubernetes Deployment and Service configuration
└── Readme.md            # Project documentation
```

## 🚀 Quick Start  

### 1️⃣ Clone the Repository  
```sh
git clone https://github.com/pikilisaikiran/simple-devops.git 
cd simple-devops  
```

### 2️⃣ Run the Flask App Locally (Optional)  
```sh
cd app  
pip install -r requirements.txt  
python app.py  
```
Visit: **http://localhost:5000**  

### 3️⃣ Build & Push Docker Image  
```sh
docker build -t your-dockerhub-username/flask-app:latest .  
docker push your-dockerhub-username/flask-app:latest  
```

### 4️⃣ Set Up Minikube & Deploy to Kubernetes  
```sh
minikube start  
kubectl apply -f k8s-deployment/flink-app.yaml  
```

### 5️⃣ Access the App in Kubernetes  
```sh
kubectl port-forward svc/flask-service 5000:5000  
```
Visit: **http://localhost:5000**  

## 📖 Full Guide  
For a step-by-step explanation, follow my Medium blog:  
👉 [Medium Blog on Deploying Flask with Docker & Kubernetes](https://medium.com/your-blog-url)  

---

## **Contributing**  
Feel free to fork this repository and make improvements. PRs are welcome!  


