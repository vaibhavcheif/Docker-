🐳 Dockerized Python Flask Application

📌 Overview
This project demonstrates how to containerize a simple Python Flask web application using Docker. It addresses common deployment challenges such as dependency conflicts, inconsistent environments, and manual setup overhead. By packaging the app into a Docker image, it ensures portability, scalability, and ease of deployment across different platforms—including Windows and Ubuntu-based EC2 servers.

🎯 Objectives

• 	✅ Create a lightweight Flask application

• 	🐳 Dockerize the app with a clean, reproducible image

• 	🚀 Run the container with a single command

• 	🌐 Access the app via browser or CLI

• 	📁 Deploy seamlessly on both Windows and EC2 Ubuntu environments

• 	🔄 Automate build and run steps with a shell script


📁 Project Structure

flask-docker-app/

├── app.py               # Flask application

├── requirements.txt     # Python dependencies

├── Dockerfile           # Docker build instructions

└── run.sh               # EC2 deployment script


🧪 How to Run

On Windows (Docker Desktop)
docker build -t flask-docker-app .
docker run -d -p 5000:5000 flask-docker-app

Visit: http://localhost:5000

On EC2 Ubuntu
chmod +x run.sh
./run.sh
Visit: http://<your-ec2-public-ip>

📦 Technologies Used
- Python 3.11
- Flask 2.3
- Docker
