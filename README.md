# Flask Docker Production Deployment

## Overview

This project demonstrates containerization and production-oriented deployment of a Flask application using Docker and Gunicorn. The focus is on creating a lightweight, reproducible, and scalable backend service.

## Tech Stack

* Python (Flask)
* Docker
* Gunicorn
* Linux

## Key Capabilities

* Containerized application using Docker
* Production-ready WSGI server (Gunicorn)
* Isolated and reproducible runtime environment
* Port-based service exposure

## Project Structure

```
app/
Dockerfile
requirements.txt
```

## Build and Run

### Clone Repository

```
git clone <repo-url>
cd flask-docker-production-deployment
```

### Build Image

```
docker build -t flask-app .
```

### Run Container

```
docker run -p 5000:5000 flask-app
```

## Output

* Application accessible at: http://localhost:5000
* Add runtime screenshots here

## Learning Outcomes

* Containerization of backend services
* Production deployment using Gunicorn
* Docker image lifecycle management

## Possible Enhancements

* Add CI/CD pipeline for automated builds
* Deploy on Kubernetes or cloud container services
* Integrate logging and monitoring
