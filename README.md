# Flask Application on Kubernetes

This repository contains a simple Flask application that is containerized using Docker and deployed on a Kubernetes cluster. It serves as a basic example of how to set up a Flask app with Kubernetes.

## Contents

- `app.py`: The main Flask application.
- `Dockerfile`: Instructions for building the Docker image of the Flask app.
- `deployment.yaml`: Kubernetes deployment configuration for the Flask application.
- `service.yaml`: Kubernetes service configuration to expose the Flask application.

## Prerequisites

- Docker installed on your machine
- Kubernetes cluster (Minikube or any cloud-based cluster)
- `kubectl` installed for interacting with the Kubernetes cluster

### Update Docker Image in Deployment File

1. Open `deployment.yaml` in a text editor.

2. Locate the following line:

   ```yaml
   image: your-dockerhub-username/flask-app:latest

3. Replace your-dockerhub-username with your actual Docker Hub username

### Steps to Edit Jenkinsfile

1. **Locate the Jenkinsfile**
   - Find the Jenkinsfile

2. **Edit the Jenkinsfile**
   - Open the Jenkinsfile in a text editor or on Github to edit

3. **Update JIRA Settings**
   - Locate lines 5 and 6 in the Jenkinsfile.
   - Replace `JIRA_SITE` with your JIRA site name. For example, if your site name is `https://sit-team-vr03pn0q.atlassian.net/`, use `sit-team-vr03pn0q`.
   - Replace `JIRA_PROJECT_KEY` with the project key you noted earlier.

   ```plaintext
   # Example:
   JIRA_SITE = "sit-team-vr03pn0q"
   JIRA_PROJECT_KEY = "YOUR_PROJECT_KEY"
   '''

4. **Update Github Link**
   - Locate line 13.
   - Replace `url` with your Github repo link (e.g. https://github.com/{github-username}/Flask_Application_Kurbenetes.git

   ```plaintext
   # Example:
   git branch: 'main', url: 'https://github.com/{github-username}/Flask_Application_Kurbenetes.git'
