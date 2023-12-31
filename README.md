# Infrastructure_Project
## Project Requirements:

#### 1- Install local K8s instance using Minikub (with Ansible).
#### 2- K8s instance will have two Namespaces: tools and dev (installed using Terraform)
#### 3- tools namespace will have pod for Jenkins and nexus(installed using Terraform)
#### 4- dev namespace will run two pods: one for nodejs application and another for MySQL DB
#### 5- Create a Jenkins pipeline job to do the following:
    Checkout code from https://github.com/Fahd-DevOps/Nodejs_App_Project.git
##### &emsp; a- Build nodejs app usng dockerfile 
##### &emsp; b- Create a Docker image
##### &emsp; c- Upload Docker image to nexus
#### 6- Create another Jenkins pipeline job that run the Docker container on the requested environment from nexus on minikube.
#### 7- Configurations of micro-services should either be handled using secrets in K8s.



## Built With
[![Terraform](https://img.shields.io/badge/Terraform-purple?style=plastic&logo=Terraform)](https://www.terraform.io/)
[![Ansible](https://img.shields.io/badge/Ansible-black?style=plastic&logo=Ansible)](https://www.ansible.com/)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-blue?style=plastic&logo=Kubernetes)](https://kubernetes.io/)
[![Docker](https://img.shields.io/badge/Docker-lightblue?style=plastic&logo=Docker)](https://www.docker.com/)
[![Jenkins](https://img.shields.io/badge/Jenkins-red?style=plastic&logo=Jenkins)](https://www.jenkins.io/)
[![Sonatype Nexus](https://img.shields.io/badge/Sonatype%20Nexus-darkgreen?style=plastic&logo=Sonatype%20Nexus)](https://www.sonatype.com/products/repository-oss)
[![Kaniko](https://img.shields.io/badge/Kaniko-blue?style=plastic&logo=Kubernetes)](https://github.com/GoogleContainerTools/kaniko)
  
- [Terraform](https://www.terraform.io) - Infrastrcuture as code
- [Ansible](https://www.ansible.com/) - Configuration Management Tool
- [Kubernetes](https://www.kubernetes.io) - Container Orchestration
- [Docker](https://www.docker.com) - Application Containerization
- [Jenkins](https://www.jenkins.io) - Automation Server For CI/CD Pipelines.
- [nexus](https://sonatype.com/) - Repository Management
- [Kaniko](https://github.com/GoogleContainerTools/kaniko/) - Container Image Builds

## Demo Description:
### Run Ansible Script: 
![Step-1](Screenshot/1.png)
### Output:
![Step-1](Screenshot/2.1.png)

![Step-1](Screenshot/2.png)


---


### Configure Jenkins: 
![Step-3](Screenshot/3.png)

---

### Jenkins Pipeline : 
![Step-4](Screenshot/12.png)

---

### Configure Nexus: 
![Step-5](Screenshot/4.png)

---

### Create Nexus Repo: 
![Step-6](Screenshot/9.png)

---

### Nexus app images: 
![Step-7](Screenshot/11.png)

---

### Config Kaniko: 
![Step-8](Screenshot/8.png)

---

### Config Kube-agent: 
![Step-9](Screenshot/7.png)

---

### Config App Deployer: 
![Step-10](Screenshot/6.png)

---

### NodeJs App: 
![Step-11](Screenshot/10.png)

## Deployment Repo for CD Stage [here](https://github.com/Fahd-DevOps/Deploy_App_Project/)

---

## Contributors:
- [Fahd Khaled](https://www.linkedin.com/in/fahd-khaled-dev/)
- [Mohamed Alaa](https://www.linkedin.com/in/mohamed-alaa-amer)
- [Mahmoud Mansour](https://www.linkedin.com/in/mahmoudmansourr/)
---
Final_Project_ITI
