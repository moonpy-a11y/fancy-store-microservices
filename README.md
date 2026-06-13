# Fancy Store E-Commerce Platform

[![Google Cloud](https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)](https://cloud.google.com/docs)
[![GKE](https://img.shields.io/badge/GKE-326CE5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)](https://cloud.google.com/kubernetes-engine/docs)
[![Microservices](https://img.shields.io/badge/Microservices-8A2BE2.svg?style=for-the-badge&logo=docker&logoColor=white)](https://cloud.google.com/learn/what-is-microservices-architecture)

Welcome to the **Fancy Store** microservices repository! This project refactors a monolithic Node.js application into a modern microservices architecture running on Google Kubernetes Engine (GKE).

## Architecture Overview

Below is the generated architecture diagram for the Fancy Store deployment:

<div align="center">
  <!-- Ensure the image is in the same directory as this README or update the relative path below -->
  <img src="./Gemini_Generated_Image_o4nc1zo4nc1zo4nc.png" alt="Fancy Store Architecture" width="800">
  <br>
</div>

##  Interactive Deployment Checklist

Click the sections below to track your deployment progress:

<details>
<summary><b>1. Containerize the Applications (Click to expand)</b></summary>
<br>

- [x] Build Monolith image (`gcloud builds submit`)
- [x] Build Orders microservice image
- [x] Build Products microservice image
- [x] Build Frontend microservice image
</details>

<details>
<summary><b>2. Provision GKE Infrastructure (Click to expand)</b></summary>
<br>

- [x] Create a 3-node Kubernetes cluster (`fancy-cluster-619`)
- [x] Authenticate `kubectl` with the new cluster
</details>

<details>
<summary><b>3. Deploy Services (Click to expand)</b></summary>
<br>

- [x] Deploy Orders Service (Port 8081)
- [x] Deploy Products Service (Port 8082)
- [x] Reconfigure Frontend `.env` with microservice IP addresses
- [x] Deploy Frontend Service (Port 8080)
</details>

## 📚 Documentation References

* **[Google Cloud Overview](https://cloud.google.com/docs)**
* **[Google Kubernetes Engine (GKE) Documentation](https://cloud.google.com/kubernetes-engine/docs)**
* **[Microservices Architecture on Google Cloud](https://cloud.google.com/learn/what-is-microservices-architecture)**

## 👨‍💻 Author
Refactored and maintained by **moonpy-ally**.

## 💻 Local Development
To run these services locally outside of GKE, ensure you have Node.js installed and run `npm install` followed by `npm start` in the respective microservice directories.
