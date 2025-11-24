# Mini DevOps Project – Docker + GitHub Actions CI/CD

---

## 📌 Project Overview
This mini DevOps project demonstrates a complete CI/CD pipeline with deployment to AWS EC2:
**Build → Dockerize → Test via GitHub Actions → Push to Docker Hub → Auto Deploy to EC2.**

---

## 🧑‍💻 Application Details
- Built a simple Node.js application
- Endpoint: `GET /hello`
- Response: `Hello from DevOps – Rohit Kamble`

---

## 🛠 Tech Stack 
- Node.js (Express)
- Docker
- Git & GitHub
- GitHub Actions (CI/CD)
- Docker Hub

---

## 🪜 Steps Completed

### Step 1: Build Application
- Created Node.js Express application with `/hello` endpoint
- Verified locally via browser & curl

### Step 2: Dockerize the Application
- Wrote a Dockerfile
- Built and ran Docker container locally
- Exposed internal port 8080
- Tested at: `http://localhost:9090/hello`

### Step 3: Push Code to GitHub
Repository includes:
- Source code (`app.js`)
- `Dockerfile`
- `.dockerignore`
- `README.md`
- GitHub Actions workflow file (`.github/workflows/ci.yml`)

### Step 4: Continuous Integration (CI) – GitHub Actions
CI workflow includes:
1. Checkout code
2. Install dependencies
3. Build Docker image
4. Run container and test `/hello`
5. Push image to Docker Hub

Trigger: on: push to master

### Step 5: Continuous Deployment (CD) – Deploy to AWS EC2
Automated deployment steps added to the same pipeline:
1. Connect to AWS EC2 via SSH (using GitHub Secrets)
2. Pull the latest image from Docker Hub
3. Remove old container (if exists)
4. Run latest container mapped to port **80 → 8080**

Access application publicly: http://<EC2-PUBLIC-IP>/hello

##  Screenshot's

![Screenshot of hello response](https://github.com/user-attachments/assets/88e2d68c-2cad-4b13-99c6-09f997ebc3b7)

![Screenshot of pipeline success](https://github.com/user-attachments/assets/91af317f-baf3-456c-a27f-c2ee4a60540e)

![CD Deployment](https://github.com/user-attachments/assets/cfae44d0-1eba-49c5-b076-77f5a269c20a)

![EC2 Display](https://github.com/user-attachments/assets/01043e42-5cb6-4515-ba6e-bd7509982295)

---

## 📦 Expected Deliverables
| Item                      | Provided |
| ------------------------- | -------- |
| GitHub Repo               | ✔        |
| Dockerfile                | ✔        |
| CI/CD Workflow            | ✔        |
| Screenshot: /hello output | ✔        |
| Screenshot: CI Success    | ✔        |
| Screenshot: CD Deployment | ✔        |
| Short Write-Up            | ✔        |

---

## 👨‍💻 Author  
Rohit Kamble

---
