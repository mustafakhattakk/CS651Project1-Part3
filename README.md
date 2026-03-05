# VisionForge AI – CS651 Project 1

VisionForge AI is a responsive startup-style web application designed to simulate an AI-powered image captioning platform.  
The website demonstrates modern web design, containerization, and cloud deployment using Docker and AWS.

This project was developed as part of **CS651 – Web Systems**.

---

# Team Members

- Mustafa Khattak
- Kokila Ganesan
- Xiaoqin Tang

---

# Project Overview

VisionForge AI allows users to upload or analyze images and generate AI-style captions, social media descriptions, and hashtags.

The goal of this project is to demonstrate:

- Frontend web development
- Responsive design with Bootstrap
- JavaScript interactivity
- Docker containerization
- Cloud deployment using AWS EC2
- Static website hosting with Amazon S3

---

# Technologies Used

Frontend

- HTML5
- CSS3
- Bootstrap
- JavaScript

Cloud & DevOps

- Docker
- DockerHub
- AWS EC2
- Amazon S3 Static Website Hosting
- GitHub

---

# Project Structure

CS651Project1
│
├── css/
├── js/
├── Images/
├── index.html
├── about.html
├── contact.html
├── dashboard.html
├── signin.html
├── Dockerfile
└── README.md

---

# Docker Containerization

The application was containerized using Docker and served through an Nginx web server.

### Build Docker Image
docker build -t visionforge-site .

### Run Docker Container
docker run -p 8080:80 visionforge-site

The application can then be accessed locally at:
http://localhost:8080

---

# DockerHub Image

The Docker image was pushed to DockerHub for deployment.

Example command:

docker push mustafakhattakk/visionforge-site:latest


---

# AWS EC2 Deployment

The Docker container was deployed to an AWS EC2 instance.

Deployment steps:

1. Launch EC2 instance
2. Configure security group (SSH + HTTP)
3. Connect via SSH
4. Install Docker
5. Pull Docker image from DockerHub
6. Run container on port 80

Example command:
docker run -d -p 80:80 mustafakhattakk/visionforge-site:latest

The website becomes publicly accessible using the EC2 public IP address.

---

# Amazon S3 Static Website Hosting (Part 3)

The website was also deployed using **Amazon S3 static website hosting**.

Deployment steps:

1. Create S3 bucket
2. Upload website files
3. Enable static website hosting
4. Configure bucket policy for public access

---

# Live Deployment

GitHub Pages
https://mustafakhattakk.github.io/CS651Project1/


---

# Demo Videos

Part 2 Deployment Video
 
https://youtu.be/qPmFDlnjC2s


Part 3 Deployment Video
https://youtu.be/qj89DWoFMGI

---

# Future Development (Project 2)

The VisionForge platform will evolve into a dynamic AI-powered web application.

Future technologies include:

- React
- Node.js
- Express
- Google Gemini API
- Firestore Database
- Google Cloud Run

---

# Course Information

Course: **CS651 – Web Systems**  
Institution: **California State University East Bay**







