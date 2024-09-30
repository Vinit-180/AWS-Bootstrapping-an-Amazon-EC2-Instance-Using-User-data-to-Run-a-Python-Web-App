# AWS Bootstrapping an Amazon EC2 Instance Using User Data to Run a Python Web App

## Project Overview
Manually setting up and configuring the packages required to run a Python web app using Nginx and uWSGI on a server can be time-consuming — and it's tough to accomplish without any errors. But why do that hard work when you can automate it?

Using AWS CDK, this project demonstrates how to set up user data scripts and an infrastructure to preconfigure an EC2 instance — transforming a manual, time-intensive process into an efficient, automated solution. The process includes deploying a Python web application from a GitHub repository using a combination of bash scripts and AWS CodeDeploy.

### Key Objectives:
- Set up an AWS CDK stack with an Amazon EC2 instance, a CI/CD Pipeline, and the required resources.
- Install software packages on the EC2 instance's first launch using a user data script.
- Deploy, test, and configure the Python web app via the CI/CD pipeline.

---

## Features
- **AWS CDK Infrastructure**: Create a stack with Amazon EC2, CodeDeploy, and other necessary resources.
- **User Data Script**: Automatically install Nginx, uWSGI, and configure the web app during the first EC2 instance launch.
- **CI/CD Pipeline**: Automate the deployment process from GitHub to the EC2 instance using AWS CodePipeline and CodeDeploy.
- **Web App Deployment**: Seamlessly deploy a Python-based web application from a GitHub repository.

---

## Prerequisites
Before getting started, ensure you have the following:
- AWS CLI installed and configured
- AWS CDK installed (`npm install -g aws-cdk`)
- Python 3.x installed
- Basic knowledge of Python, AWS, and infrastructure automation

---

## Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/Vinit-180/AWS-Bootstrapping-an-Amazon-EC2-Instance-Using-User-data-to-Run-a-Python-Web-App.git
cd AWS-Bootstrapping-an-Amazon-EC2-Instance-Using-User-data-to-Run-a-Python-Web-App
```
### 2. Bootstrap your AWS Environment
```bash
cdk bootstrap
```

### 3. Deploy the CDK Stack
```bash
cdk deploy
```

### 4. Check Deployment & Access the Web App
After deployment, grab the public IP of the EC2 instance and access the Python web app through the browser.


### Technologies Used
- **Python**: Backend language for the web app
- **Amazon Web Services (AWS)** : EC2, CodeDeploy, CodePipeline, CDK, S3
- **Nginx** : Web server to serve the Python application
- **AWS CDK**: For infrastructure-as-code to automate EC2 setup
