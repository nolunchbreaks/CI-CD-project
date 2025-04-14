# CI/CD Flask Web Application with Docker

## Overview

This project demonstrates the setup of a **Flask web application** with a **CI/CD pipeline**, using **Docker** for containerization. It is a simple web application that allows for easy development, testing, and deployment in an automated fashion.

The project integrates:
- **Flask** for the backend web framework.
- **HTML** for the frontend user interface.
- **Docker** for containerizing the application.
- **CI/CD Pipeline** for automated testing, building, and deployment.

## Features

- **Flask Web Application**: A basic Flask-based web application serving HTML content.
- **HTML Frontend**: A simple HTML interface to interact with the Flask backend.
- **Docker**: Containerized environment to ensure the application runs seamlessly across different environments.
- **CI/CD Pipeline**: Automated processes for testing, building, and deploying the app using a CI/CD tool (e.g., GitHub Actions, Jenkins, or GitLab CI).

## Technologies Used

- **Flask**: Python web framework for building the backend API.
- **HTML**: Frontend markup for displaying content.
- **Docker**: Containerization for packaging the application.
- **CI/CD Tool**: GitHub Actions (or another CI/CD tool) for automating the build, test, and deployment process.
- **Python 3.x**: Backend programming language.
- **Git**: Version control for the project.

## Getting Started

### Prerequisites

- Python 3.6 or higher
- Docker installed on your machine
- A CI/CD platform (e.g., GitHub Actions, Jenkins, GitLab CI)

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/cicd-flask-docker.git
    cd cicd-flask-docker
    ```

2. Install the required dependencies locally (optional, but recommended):

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    pip install -r requirements.txt
    ```

### Running the Application Locally

To run the Flask application locally without Docker, use the following commands:

1. Start the Flask application:

    ```bash
    flask run
    ```

2. Open your browser and visit `http://127.0.0.1:5000` to see the web application.

### Running with Docker

To run the application in a Docker container, follow these steps:

1. Build the Docker image:

    ```bash
    docker build -t flask-cicd-app .
    ```

2. Run the Docker container:

    ```bash
    docker run -p 5000:5000 flask-cicd-app
    ```

3. Open your browser and visit `http://127.0.0.1:5000` to view the application running inside the Docker container.

### CI/CD Pipeline

1. The project comes with a sample GitHub Actions pipeline (or your CI/CD platform of choice) located in `.github/workflows/ci-cd.yml` (or corresponding directory for other platforms).
2. When you push changes to the repository, the CI/CD pipeline will automatically trigger:
    - **Test**: Run unit tests on the Flask application.
    - **Build**: Build the Docker image for the application.
    - **Deploy**: Deploy the application (to a server or cloud service).

## How It Works

- **Flask Backend**: The application serves dynamic content through Flask, listening on port 5000.
- **Docker Containerization**: The Flask application is containerized using Docker to ensure it runs consistently across different environments.
- **CI/CD Pipeline**: The pipeline automates the process of testing, building, and deploying the application each time changes are pushed to the repository.

## Customization

You can easily extend this project by:
- Modifying the `app.py` file for additional Flask routes and functionality.
- Adding more HTML pages or static files in the `templates/` and `static/` directories.
- Customizing the `Dockerfile` and CI/CD configuration files to fit your deployment platform.

## License

This project is open-source and available under the MIT License.
