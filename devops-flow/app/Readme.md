# Flask App for DevOps Demo  

This is a simple **Flask web application** that responds with a message when accessed.  

## 🛠️ Running Locally  
```sh
pip install -r requirements.txt  
python app.py  
```
Visit: **http://localhost:5000**  

## 🐳 Running in Docker  
```sh
docker build -t flask-app .  
docker run -p 5000:5000 flask-app  
```

## 📦 Dependencies  
- Flask  

## 📌 Notes  
- The app runs on **port 5000** by default.  
