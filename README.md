# CI/CD Deployment with Jenkins (Flask + Express)

## Overview
This project demonstrates deploying a Flask backend and an Express frontend on a single AWS EC2 instance with a Jenkins CI/CD pipeline.

## Architecture
<img width="1025" height="640" alt="Screenshot-19" src="https://github.com/user-attachments/assets/9bed88fb-3123-4fbf-b692-19d647cd693f" />


## Technologies Used
- AWS EC2
- Jenkins
- Python (Flask)
- Node.js (Express)
- PM2
- GitHub

## Deployment Steps
1. Provision EC2 instance
2. Install dependencies (Python, Node.js, Git, Jenkins)
3. Clone repositories
4. Run Flask on port 5000 and Express on port 3000
5. Set up Jenkins pipelines for automated deployment

## Verification
- Flask: http://13.232.79.50:5000
- Express: http://13.232.79.50:3000

## Jenkins Automation
Each push to the main branch triggers a Jenkins pipeline that:
- Pulls latest code
- Installs dependencies
- Restarts the application via PM2
