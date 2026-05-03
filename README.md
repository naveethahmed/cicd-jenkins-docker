# 🚀 CI/CD Pipeline using Jenkins and Docker

## 📌 Overview
Automated CI/CD pipeline that builds and deploys a Dockerized 
web application on AWS EC2 using Jenkins.

## 🏗️ Pipeline Flow
GitHub Push → Jenkins Trigger → Docker Build → Deploy on EC2

## 🛠️ Tools & Technologies
| Tool | Purpose |
|------|---------|
| Jenkins | CI/CD Automation |
| Docker | Containerization |
| GitHub | Source Code Management |
| AWS EC2 | Cloud Hosting (ap-south-1) |
| Nginx | Web Server |

## ⚙️ Pipeline Stages
1. **Clone** - Pull code from GitHub repository
2. **Build** - Build Docker image from Dockerfile
3. **Deploy** - Run container on EC2 instance
4. **Verify** - Confirm container is running

## 📂 Project Structure
cicd-jenkins-docker/
├── Jenkinsfile       # Pipeline configuration
├── Dockerfile        # Container build instructions
├── index.html        # Web application
└── README.md         # Project documentation

## 🚀 How to Run Locally
```bash
# Clone the repository
git clone https://github.com/naveethahmed/cicd-jenkins-docker

# Build Docker image
docker build -t myapp:latest .

# Run container
docker run -d -p 80:80 myapp:latest

# Open browser
http://localhost:80
```

## 👨‍💻 Author
**Naveeth Ahmed N** | DevOps Engineer  
📧 naveethahmedn@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/naveeth-ahmed-a44181313)
