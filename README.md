# DevOps Portfolio 

A practical DevOps portfolio demonstrating CI/CD pipelines, container orchestration, stateful storage, and monitoring — all built from real-world exercises and production-style workflows.

---

## 🧰 Tech Stack

| Category | Tools & Technologies |
|-----------|----------------------|
| **Languages & Scripting** | Bash, YAML, Python, Groovy |
| **Version Control** | Git, GitHub, Gitea |
| **CI/CD** | Jenkins, GitHub Actions |
| **Containers & Orchestration** | Docker, Kubernetes, Helm |
| **Monitoring & Logging** | Prometheus, Grafana |
| **Cloud & Infrastructure** | AWS (EC2, S3, IAM), Azure Fundamentals |
| **Security & Secrets Management** | TLS, SSH, Vault, Kubernetes Secrets |
| **OS & Environments** | Linux (Ubuntu, CentOS), Windows Server |


---

## 🚀 Featured Projects

| Project | Description | Folder |
|----------|--------------|---------|
| **Jenkins Auto-Deploy** | Automates build and deployment of a static web app using Jenkins pipelines and SSH. | [`Jenkins/`](./Jenkins) |
| **Kubernetes Guestbook** | Redis master–replica setup using Deployments and Services. | [`Kubernetes/guestbook`](./Kubernetes/guestbook) |
| **MySQL with PVC + Secret** | Persistent and secure DB deployment using Kubernetes PVC and Secret. | [`DB/mysql`](./DB/mysql) |
| **Monitoring Stack** | Prometheus + Grafana installation via Helm chart. | [`Monitoring/prometheus-grafana`](./Monitoring/prometheus-grafana) |

---
## 🧱 Project Structure

| Component | Description | Path |
|------------|-------------|------|
| Jenkins | CI/CD pipeline jobs and automation | [Jenkins/job/](./Jenkins/job/) |
| Kubernetes | Guestbook app deployment (frontend + backend) | [Kubernetes/guestbook/](./Kubernetes/guestbook/) |
| Database (MySQL) | Persistent MySQL setup using PVC and Secrets | [DB/mysql/](./DB/mysql/) |
| Monitoring | Prometheus + Grafana via Helm | [Monitoring/prometheus-grafana/](./Monitoring/prometheus-grafana/) |

---

## 🌐 Live Project Links

## 🧩 How to Run Locally
git clone https://github.com/Mictwito/DevOps-Portfolio.git
cd Kubernetes/guestbook && kubectl apply -f .

### 🧩 Jenkins Pipeline
- [📂 View Files](./Jenkins/job/)
- [▶️ Open in Cloud Shell](https://shell.cloud.google.com/?repo=https://github.com/Mictwito/DevOps-Portfolio.git&dir=Jenkins/job)
- > _Run inside Cloud Shell:_  
> `jenkins-jobs build all`



### ☸️ Kubernetes Guestbook
- [📂 View Files](./Kubernetes/guestbook/)
- [▶️ Open in Cloud Shell](https://shell.cloud.google.com/?repo=https://github.com/Mictwito/DevOps-Portfolio.git&dir=Kubernetes/guestbook)
- > _Run inside Cloud Shell:_  
> `kubectl apply -f . && kubectl get pods,svc`
>
> 

### 🗄️ MySQL Database
- [📂 View Files](./DB/mysql/)
- [▶️ Open in Cloud Shell](https://shell.cloud.google.com/?repo=https://github.com/Mictwito/DevOps-Portfolio.git&dir=DB/mysql)
- > _Run inside Cloud Shell:_  
> `kubectl apply -f DB/mysql/`




### 📊 Monitoring (Prometheus + Grafana)
- [📂 View Files](./Monitoring/prometheus-grafana/)
- [▶️ Open in Cloud Shell](https://shell.cloud.google.com/?repo=https://github.com/Mictwito/DevOps-Portfolio.git&dir=Monitoring/prometheus-grafana)
- > _Run inside Cloud Shell:_  
> `helm install monitoring ./Monitoring/prometheus-grafana`



---

## 📊 GitHub Stats
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Mictwito&show_icons=true&theme=tokyonight)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Mictwito&layout=compact&theme=tokyonight)

---

## 🧭 About Me
I’m a hands-on DevOps Engineer passionate about automation, infrastructure, and continuous delivery.  
I enjoy building efficient, secure, and scalable systems — always learning, always improving.  
This portfolio reflects my progress through 100 days of practical DevOps labs, including CI/CD, Kubernetes, monitoring, and system automation.

---

## 📫 Connect
- **GitHub:** [github.com/Mictwito](https://github.com/Mictwito)


---

