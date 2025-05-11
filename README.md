# 🚀 DevOps Pipeline with Google Cloud CI/CD

_A tutorial by **Aditya Saxena**_

---

## 📘 Overview

In this lab, you will build a complete **Continuous Integration (CI) pipeline** using:
- **Cloud Source Repositories** (Git-based source control)
- **Cloud Build** (automated build and test platform)
- **Artifact Registry** (Docker image repository)
- **Build Triggers** (event-driven automation)

You will also create, containerize, and deploy a simple **Flask web app** using Google Cloud-native services.

![DevOps Pipeline](../DevOps_Pipeline.png)
---

## 🎯 Objectives

By the end of this tutorial, you will be able to:

- ✅ Create a Git repository in Cloud Source Repositories  
- ✅ Develop and test a Python web application using Flask  
- ✅ Define and build Docker containers  
- ✅ Store container images in Artifact Registry  
- ✅ Automate Docker builds using Cloud Build and triggers  
- ✅ Deploy and test your application on Compute Engine  

---

## 🧪 Prerequisites & Setup

- A Google Cloud Platform (GCP) project with billing enabled
- IAM permissions to create resources: Cloud Source Repos, Cloud Build, Artifact Registry, Compute Engine
- Access to **Cloud Shell** and **Cloud Console**

---

## 🛠️ Tasks Breakdown

### 🔹 Task 1: Create a Git Repository
- Use **Cloud Source Repositories** to create `devops-repo`
- Clone the repo in **Cloud Shell**
- Organize your project folder `~/gcp-course/devops-repo`

---

### 🔹 Task 2: Create a Simple Python Flask App
- Create `main.py` with a simple web route
- Add `templates/layout.html` and `templates/index.html`
- Add `requirements.txt` for dependencies
- Commit and push changes to `devops-repo`

---

### 🔹 Task 3: Define a Docker Build
- Create a `Dockerfile` to containerize your app
- Use **Gunicorn** as the production web server
- Define working directory, install dependencies, expose port

---

### 🔹 Task 4: Manage Images with Cloud Build & Artifact Registry
- Create Docker image repository `devops-repo`
- Authenticate Docker to GCP
- Use `gcloud builds submit` to:
  - Build Docker image
  - Store it in Artifact Registry
- View image in Artifact Registry UI

---

### 🔹 Task 5: Automate Builds with Triggers
- Create a build trigger using Cloud Build
- Use an **inline `cloudbuild.yaml`** to define Docker build steps
- Trigger builds on every push to `master`
- Commit a small code change and verify automated build

---

### 🔹 Task 6: Test Your Build Changes
- Deploy your image to a **Compute Engine VM**
- Use **"Deploy Container"** option and paste Docker image URI
- Access your app via external IP
- Confirm that the updated message is visible in the browser

---

## 📦 Key Services Used

| GCP Service         | Purpose                             |
|---------------------|-------------------------------------|
| Cloud Source Repos  | Version control system (Git)        |
| Cloud Build         | Build and CI automation             |
| Artifact Registry   | Docker image hosting                |
| Compute Engine      | Deploy and run your app             |

---

## 🧠 Final Notes

- This pipeline is the foundation of modern **cloud-native DevOps**.
- Easily extend this with:
  - **Cloud Run** or **GKE** for serverless/container orchestration
  - **Cloud Monitoring & Logging**
  - **Security scanners** (e.g., Trivy)

---

## 🏁 Congratulations!

You've completed a full DevOps CI pipeline from code to container to deployment on Google Cloud. 🚀

---

## 👨‍🏫 Instructor

**Aditya Saxena**  
Professor & Cloud DevOps Engineer  
[LinkedIn Profile](https://www.linkedin.com/in/itsadisxnn)# GCP_DevOps_Pipeline
