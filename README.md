# nodejs-demo-app
this repository contains a demo Node.js application for ElivateLabs.  
It demonstrates a basic Node.js setup, routing, Docker containerization, and CI/CD pipeline integration using GitHub Actions.

## Table of Contents
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Docker](#docker)
- [GitHub Actions CI/CD](#github-actions-cicd)

Install packages
```
npm install
```
Start server
```
npm start
````
URL Browser

```
http://localhost:5000/

```
GitHub Actions CI/CD

This project can automatically build and push Docker images using GitHub Actions.

Setup Secrets in GitHub

Go to your repository → Settings → Secrets → Actions, and add:

            DOCKERHUB_USERNAME – Your Docker Hub username

            DOCKERHUB_TOKEN – Docker Hub access token

            DOCKER_REGISTRY – Your Docker Hub username

            DOCKER_IMAGE – Desired image name

Workflow Behavior:
     -Triggered on push or pull request to the main branch.
     -Builds the Docker image and pushes it to Docker Hub.
     -Tags the Docker image with the GitHub run number for versioning.
