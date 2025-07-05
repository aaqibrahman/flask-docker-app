# 🐳 Dockerized Flask Web App

A simple Flask application containerized with Docker and pushed to Docker Hub.

---

## 🚀 Project Goals

- Learn containerization basics using Docker  
- Build and run a simple Flask web app in a Docker container  
- Push the Docker image to Docker Hub

---

## 🧰 Tech Stack

- Python 3.9  
- Flask  
- Docker  
- Docker Hub  

---

## 📁 Project Structure
flask-docker-app/  
├── app.py # Main Flask app\  
├── requirements.txt # Python dependencies\  
└── Dockerfile # Docker image configuration\

### Clone the Repository
git clone https://github.com/yourusername/flask-docker-app.git<br>
cd flask-docker-app<br>

## Build the Docker Image

docker build -t yourdockerhubusername/flask-docker-app .<br>
(Replace yourdockerhubusername with your actual Docker Hub username.)

## Run the Container Locally
docker run -p 5000:5000 yourdockerhubusername/flask-docker-app<br>
Visit http://localhost:5000 in your browser.

## 📤 Push to Docker Hub
# Log in to Docker Hub
docker login

# Tag and Push the Image
docker tag flask-docker-app yourdockerhubusername/flask-docker-app<br>
docker push yourdockerhubusername/flask-docker-app
# ✅ Output
You should see:<br>
Hello from Dockerized Flask App!<br>
in your browser at localhost:5000.

# 🧼 To Stop the Container
Find the container ID:<br>
docker ps<br>
Then stop it:<br>
docker stop <container_id>


# 📦 Pulling the Image (from another machine)
docker pull yourdockerhubusername/flask-docker-app<br>
docker run -p 5000:5000 yourdockerhubusername/flask-docker-app<br>


