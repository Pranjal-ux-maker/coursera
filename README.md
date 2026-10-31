# Python CI/CD Pipeline using GitHub Actions and OpenShift Tekton

## Project Description

This project demonstrates the implementation of a Continuous Integration and Continuous Deployment (CI/CD) pipeline using GitHub Actions and OpenShift Tekton.

The pipeline automates code quality checks, unit testing, and pipeline execution to ensure reliable software delivery.

## Technologies Used

- **Python** – Application development
- **GitHub** – Source code management
- **GitHub Actions** – Continuous Integration
- **Flake8** – Python code linting
- **Nose** – Unit testing
- **OpenShift** – Container application platform
- **Tekton** – CI/CD pipeline automation
- **PersistentVolumeClaim (PVC)** – Persistent storage management

## Project Structure

```text
my-final-project/
│
├── README.md
├── app.py
├── test_app.py
├── requirements.txt
│
├── .github/
│   └── workflows/
│       └── workflow.yml
│
└── .tekton/
    └── tasks.yml
```

## Features

1. Automated code quality checking using Flake8.
2. Automated unit testing using Nose.
3. GitHub Actions workflow for Continuous Integration.
4. Tekton tasks for workspace cleanup and unit testing.
5. OpenShift pipeline execution.
6. Persistent storage configuration using PVC.
7. Application monitoring through OpenShift logs.

## Installation and Setup

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd my-final-project
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the Application

```bash
python app.py
```

### 4. Run Code Quality Check

```bash
flake8 .
```

### 5. Run Unit Tests

```bash
nosetests
```

## CI/CD Pipeline Workflow

The project follows these stages:

1. Developer pushes code to GitHub.
2. GitHub Actions automatically triggers the workflow.
3. Python dependencies are installed.
4. Flake8 checks the code quality.
5. Nose executes unit tests.
6. Tekton performs workspace cleanup.
7. Tekton executes unit tests in OpenShift.
8. Pipeline execution status is verified.

## OpenShift Configuration

The OpenShift environment is used to execute the Tekton pipeline.

The pipeline consists of:

- Cleanup Task
- Unit Testing Task
- PersistentVolumeClaim for workspace storage

## Expected Outcome

The project aims to achieve:

- Successful GitHub Actions workflow execution.
- Successful linting and unit testing.
- Successful OpenShift Tekton pipeline execution.
- Verified persistent storage configuration.
- Successful application deployment and accessible application logs.

## Author

**Name:** Your Name

**Project:** CI/CD Pipeline Implementation

**Academic Submission:** Final Project
