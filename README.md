# CI/CD Dashboard Flask App and My Portfolio

## Overview

This project demonstrates the setup of a **Flask web application** with a **CI/CD pipeline**, using **Docker** for containerization. It is a simple web application that includes two main pages: a **Dashboard** and a **Portfolio**. The project automates the testing, building, and deployment process through CI/CD.

The project integrates:
- **Flask** for the backend web framework.
- **HTML** for the frontend user interface, including **Dashboard** and **Portfolio** pages.
- **Docker** for containerizing the application.
- **CI/CD Pipeline** for automated testing, building, and deployment.

## Features

- **Flask Web Application**: A basic Flask-based web application serving dynamic content.
- **Dashboard Page**: A page displaying key metrics or stats, usually for administrative purposes.
- **Portfolio Page**: A page showcasing my work, achievements, and projects.
- **Docker**: Containerized environment to ensure the application runs seamlessly across different environments.
- **CI/CD Pipeline**: Automated processes for testing, building, and deploying the app using a CI/CD tool (e.g., GitHub Actions, Jenkins, or GitLab CI).

## Technologies Used

- **Flask**: Python web framework for building the backend API.
- **HTML**: Frontend markup for displaying content (including Dashboard and Portfolio pages).
- **Docker**: Containerization for packaging the application.
- **CI/CD Tool**: GitHub Actions (or another CI/CD tool) for automating the build, test, and deployment process.
- **Python 3.x**: Backend programming language.
- **Git**: Version control for the project.

## Getting Started

### Prerequisites

- Python 3.6 or higher
- Docker installed on your machine
- A CI/CD platform (e.g., GitHub Actions, Jenkins, GitLab CI)

### CI/CD Pipeline

1. The project comes with a sample GitHub Actions pipeline (or your CI/CD platform of choice) located in `.github/workflows/ci-cd.yml` (or corresponding directory for other platforms).
2. When you push changes to the repository, the CI/CD pipeline will automatically trigger:
    - **Test**: Run unit tests on the Flask application.
    - **Build**: Build the Docker image for the application.
    - **Deploy**: Deploy the application (to a server or cloud service).

## Application Pages

### Dashboard Page

The **Dashboard** page is an overview page typically used for displaying key information or stats. It can be used by administrators to monitor various metrics, or as an overview of the application.

### Portfolio Page

The **Portfolio** page showcases my  work, achievements, and projects. 

- **Location**: `templates/dashboard.html`, `templates/portfolio.html`

## How It Works

- **Flask Backend**: The application serves dynamic content through Flask, listening on port 5000.
- **Docker Containerization**: The Flask application is containerized using Docker to ensure it runs consistently across different environments.
- **CI/CD Pipeline**: The pipeline automates the process of testing, building, and deploying the application each time changes are pushed to the repository.

## Customization

You can easily extend this project by:
- Modifying the `app.py` file for additional Flask routes and functionality.
- Adding more HTML pages or static files in the `templates/` and `static/` directories (e.g., `dashboard.html`, `portfolio.html`).
- Customizing the `Dockerfile` and CI/CD configuration files to fit your deployment platform.

## License

This project is open-source and available under the MIT License.
