
# Jenkins CI/CD Pipeline for Flask Application

This repository demonstrates the setup of a Continuous Integration and Continuous Deployment (CI/CD) pipeline for a Python Flask web application using Jenkins. The pipeline automates the stages of building, testing, and deploying the application.

## Table of Contents
- [Project Overview](#project-overview)
- [Prerequisites](#prerequisites)
- [Pipeline Workflow](#pipeline-workflow)
- [Project Structure](#project-structure)
- [Setup Guide](#setup-guide)


## Project Overview
This project uses Jenkins to build a CI/CD pipeline that automates testing and deployment for a simple Flask application. The pipeline performs the following steps:
1. **Build** - Installs dependencies.
2. **Test** - Runs unit tests for the application.
3. **Deploy** - Deploys the application to a production server or local environment.

## Prerequisites
To run this pipeline, ensure you have the following:
- **Jenkins** installed and configured.
- **Python 3.8+** installed.
- **Git** installed for repository management.
- **Flask** installed as the application framework.
- A configured **Jenkins Job** with access to this repository.
- **An EKS Cluster** to Deploy the Application.
- **Domain** to To access the Loadbalancer endpoint securily.

## Pipeline Workflow
The pipeline consists of the following stages:
1. **Clone Repository** - Clones this GitHub repository.
2. **Install Dependencies** - Uses `pip` to install dependencies specified in `requirements.txt`.
3. **Run Tests** - Executes unit tests to validate application integrity.
4. **Build and Deploy** - Deploys the Flask application on a target environment.

## Install Dependencies
pip install -r requirements.txt


### Coming Features:
- SMS / Email code verification
- QR code authentication sync

## Demo
<img width="50%" src="/assets/login.JPG" alt="login">
<img width="50%" src="/assets/verify.JPG" alt="verify">
<img width="50%" src="/assets/2facode.JPG" alt="verify">

## Flask
### Localhost
```python -m flask run```
```http://127.0.0.1:5000```
### For Using LoadBalancer and DNS
```lucky1225.blog/falsk```
