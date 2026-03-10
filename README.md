# Dockerized Flask Application

## Overview

This project demonstrates how to containerize a simple Flask web application using Docker. The application runs inside a Docker container and can be accessed through a web browser using port mapping.

The purpose of this project is to understand the Docker workflow, including building images, running containers, and managing the container lifecycle.

---

## Technologies Used

* Python
* Flask
* Docker
* Ubuntu

---

## Project Structure

```
docker-flask-app
│
├── Dockerfile
├── app.py
├── requirements.txt
└── README.md
```

---

## Application Description

The Flask application is a minimal web server that returns a simple message when accessed through the browser.

Example output:

```
Hello from Docker Container!
```

---

## Dockerfile Explanation

The Dockerfile defines how the application container image is built.

* **FROM python:3.10** – Uses the official Python base image.
* **WORKDIR /app** – Sets the working directory inside the container.
* **COPY . /app** – Copies project files into the container.
* **RUN pip install -r requirements.txt** – Installs application dependencies.
* **EXPOSE 5000** – Exposes port 5000 for external access.
* **CMD ["python", "app.py"]** – Starts the Flask application.

---

## How to Run the Project

### Build the Docker Image

```
docker build -t flask-docker-app .
```

### Run the Docker Container

```
docker run -d -p 5000:5000 flask-docker-app
```

### Access the Application

Open the browser and visit:

```
http://localhost:5000
```

---

## Docker Commands Used

| Command      | Description                            |
| ------------ | -------------------------------------- |
| docker build | Build a Docker image from a Dockerfile |
| docker run   | Run a container from an image          |
| docker ps    | List running containers                |
| docker logs  | View container logs                    |
| docker stop  | Stop a running container               |
| docker rm    | Remove a container                     |
| docker rmi   | Remove a Docker image                  |

---

## Learning Outcomes

* Understanding containerization concepts
* Writing and structuring a Dockerfile
* Building Docker images
* Running containers and mapping ports
* Managing containers using Docker commands

---

## Author

Sanyam Jain
MCA Student | Cloud Computing Enthusiast
