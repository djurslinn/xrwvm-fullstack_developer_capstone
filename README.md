# fullstack_developer_capstone


## Overview

This project is a Full Stack Developer Capstone application that demonstrates the development, deployment, and management of a modern web application using frontend technologies, backend services, databases, containers, and cloud-native deployment practices.

The application provides dealership management functionality, allowing users to browse dealerships, view dealer information, and interact with backend services through a RESTful architecture.

## Features

* Dealership listing and management
* Dealer details and reviews
* REST API integration
* Database-backed application
* Containerized deployment with Docker
* Kubernetes deployment support
* CI/CD integration with GitHub
* Responsive user interface

## Project Structure

```text
xrwvm-fullstack_developer_capstone/
│
├── .github/                 # GitHub workflows and configuration
├── server/                  # Backend application source code
├── README.md                # Project documentation
├── LICENSE                  # License file
└── .gitignore               # Git ignore configuration
```

## Technologies Used

### Frontend

* HTML5
* CSS3
* JavaScript
* React

### Backend

* Python
* Django
* Django REST Framework

### Database

* SQLite
* PostgreSQL (Deployment Ready)

### DevOps & Deployment

* Docker
* Kubernetes
* GitHub Actions
* IBM Cloud Code Engine

## Installation

### Clone Repository

```bash
git clone https://github.com/djurslinn/xrwvm-fullstack_developer_capstone.git
cd xrwvm-fullstack_developer_capstone
```

### Backend Setup

```bash
cd server

python -m venv env

source env/bin/activate
# Windows
# env\Scripts\activate

pip install -r requirements.txt
```

### Database Migration

```bash
python manage.py migrate
```

### Run Development Server

```bash
python manage.py runserver
```

The application will be available at:

```text
http://127.0.0.1:8000/
```

## Docker Deployment

Build Docker Image:

```bash
docker build -t dealership-app .
```

Run Container:

```bash
docker run -p 8000:8000 dealership-app
```

## Kubernetes Deployment

Apply Kubernetes resources:

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

Verify deployment:

```bash
kubectl get deployments
kubectl get pods
kubectl get services
```

Port Forward:

```bash
kubectl port-forward deployment/dealership 8000:8000
```

## API Endpoints

| Endpoint     | Method | Description             |
| ------------ | ------ | ----------------------- |
| /dealers     | GET    | Retrieve dealerships    |
| /dealer/{id} | GET    | Retrieve dealer details |
| /reviews     | GET    | Retrieve reviews        |
| /add_review  | POST   | Add a review            |

## Future Enhancements

* User authentication
* Dealer administration panel
* Advanced filtering and search
* Review moderation system
* Analytics dashboard

## License

This project is licensed under the MIT License.

## Author

Developed as part of the Full Stack Developer Capstone Project.
