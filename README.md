# Mini DevOps Project – Docker + GitHub Actions CI/CD

--- 
## Project Overview
## This mini DevOps project follows a complete CI/CD workflow:
### Build a simple application → Dockerized it → Deploy CI pipeline using GitHub Actions.

---

## Application Details
### Simple Node.js web application with one endpoint:  **GET /hello**

### Response: Hello from DevOps – Rohit Kamble

---

## 🛠 Tech Stack 
- Node.js (Express)
- Docker
- Git & GitHub
- GitHub Actions (CI/CD)
- Docker Hub

---

## 🪜 Steps Completed

### **Step 1: Build a Simple Application**
- Created a Node.js Express server
- Implemented `/hello` endpoint
- Tested successfully via browser

### **Step 2: Dockerized the Application**
- Created a Dockerfile and built an image
- Exposed container port **8080**
- Ran container locally using:

```bash
docker build -t devops-hello-app .
```

```bash
docker run -d -p 9090:8080 --name devops-hello-container devops-hello-app
```
- Tested URL
```bash
http://localhost:9090/hello
```
### **Step 3: Push Code to GitHub**
- Application source code
- Dockerfile
- .docker ignore
- GitHub Actions CI pipeline file (.github/workflows/ci.yml)

### **Step 4: Set up CI/CD using GitHub Actions**
#### Pipeline processes:
- Checkout repository code
- Install dependencies
- Build Docker image
- Run Docker container
- Test /hello endpoint via curl
- (Bonus) Push Docker image to Docker Hub

---
###  **🔗** GitHub repo link
### https://github.com/RohitKamble14/Mini-DevOps-Project.git


### **🔗** CI pipeline file

![[ci 1.yml]]

---
##  Screenshot's

![Screenshot of hello response](https://github.com/user-attachments/assets/88e2d68c-2cad-4b13-99c6-09f997ebc3b7)

![Screenshot of pipeline success](https://github.com/user-attachments/assets/91af317f-baf3-456c-a27f-c2ee4a60540e)

---
## 📦 Expected Deliverables
| Deliverable                     | Status     |
| ------------------------------- | ---------- |
| GitHub Repo Link                | ✔ Provided |
| CI Pipeline File                | ✔ Included |
| Screenshot: Pipeline success    | ✔ Provided |
| Screenshot: `/hello` response   | ✔ Provided |
| Short write-up describing steps | ✔ Included |

---
## 👨‍💻 Author  

Rohit Kamble

---
