# Node.js CI/CD Pipeline using GitHub Actions and Docker

This repository contains a sample Node.js application configured with a complete CI/CD automation pipeline for the Elevate Labs DevOps Internship Task 1

## 📋 Task Overview
* **Objective**: Set up a CI/CD pipeline to build and deploy a web application using automation
* 
* **Tools Used**: GitHub, GitHub Actions, Node.js, Docker, and DockerHub
* 
* **Deliverable**: GitHub repository featuring the `.yml` CI/CD workflow and project source files

---

## 🛠️ Project Structure
* `app.js`: A simple Node.js HTTP server responding with `Hello from Node.js CI/CD Demo!`.
* `test.js`: Built-in Node.js test script (`node --test`) verifying core application logic.
* `Dockerfile`: Containerizes the Node.js application using a lightweight `node:20-alpine` base image.
* `.dockerignore`: Excludes unnecessary files like `node_modules` and `.git` from the Docker build context.
* `.github/workflows/main.yml`: Defines the automation pipeline.

---

## ⚙️ CI/CD Pipeline Workflow
The pipeline triggers automatically on every push to the `main` branch and runs two automated jobs

1. **`test`**: Sets up the Node.js environment, installs dependencies, and runs the test suite (`npm test`).
2. **`build-and-push`**: Authenticates securely using GitHub Secrets (`DOCKER_USERNAME` and `DOCKER_PASSWORD`), builds the Docker image, and pushes it directly to DockerHub

---

## 🚀 Verification & Links
* **GitHub Actions**: Verified via successful workflow runs (Green Ticks `✔`) in the Actions tab.
* **DockerHub Repository**: Deployed and available at [kishore2406/nodejs-demo-app](https://hub.docker.com/r/kishore2406/nodejs-demo-app)
  
