# Node.js CI/CD Pipeline using GitHub Actions and Docker

This repository contains a sample Node.js application configured with a complete CI/CD automation pipeline for the Elevate Labs DevOps Internship Task 1[span_0](start_span)[span_0](end_span).

## 📋 Task Overview
* **Objective**: Set up a CI/CD pipeline to build and deploy a web application using automation[span_1](start_span)[span_1](end_span).
* **Tools Used**: GitHub, GitHub Actions, Node.js, Docker, and DockerHub[span_2](start_span)[span_2](end_span).
* **Deliverable**: GitHub repository featuring the `.yml` CI/CD workflow and project source files[span_3](start_span)[span_3](end_span).

---

## 🛠️ Project Structure
* `app.js`: A simple Node.js HTTP server responding with `Hello from Node.js CI/CD Demo!`.
* `test.js`: Built-in Node.js test script (`node --test`) verifying core application logic.
* `Dockerfile`: Containerizes the Node.js application using a lightweight `node:20-alpine` base image.
* `.dockerignore`: Excludes unnecessary files like `node_modules` and `.git` from the Docker build context.
* `.github/workflows/main.yml`: Defines the automation pipeline.

---

## ⚙️ CI/CD Pipeline Workflow
The pipeline triggers automatically on every push to the `main` branch and runs two automated jobs[span_4](start_span)[span_4](end_span):
1. **`test`**: Sets up the Node.js environment, installs dependencies, and runs the test suite (`npm test`).
2. **`build-and-push`**: Authenticates securely using GitHub Secrets (`DOCKER_USERNAME` and `DOCKER_PASSWORD`), builds the Docker image, and pushes it directly to DockerHub[span_5](start_span)[span_5](end_span).

---

## 🚀 Verification & Links
* **GitHub Actions**: Verified via successful workflow runs (Green Ticks `✔`) in the Actions tab.
* **DockerHub Repository**: Deployed and available at [kishore2406/nodejs-demo-app](https://hub.docker.com/r/kishore2406/nodejs-demo-app)[span_6](start_span)[span_6](end_span).
  
