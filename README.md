# DevSecOps Project: Deploy Netflix on Kubernetes.

## Introduction
<div align="justify"> DevSecOps Project to setup Netflix clone on AWS using CICD, Security, Monitoring and GitOps. In this project I'm going to create my own Netflix application using DevSecOps practices which will include CI/CD using Jenkins, monitoring using Prometheus and Grafana, security using SonarQube and Trivy. More along with this, we are also going to use Argo CD and Helm to deploy the application in kubernetes.</div> <br>

_You can view the technical documentation here: [DevSecOps Project Technical Documentation](https://github.com/JavierRamirezMoral/DevSecOps-Project-Netflix/blob/main/DOCUMENTACI%C3%93N/JavierRam%C3%ADrezMoral%20DevSecOps%20Project%20-%20Deploy%20Netflix%20on%20Kubernetes.pdf)_


## Design
* We start with creating an E2 instance and deploying our application locally using Docker container. Clone my GitHub repository in the EC2 instance.
* Once the application is running, we are going to integrate security using SonarQube and Trivy.
* Once it is done manually, we are going to automate this process using a CI/CD tool Jenkins. Is going to automate creation of Docker image which is going to be secured and uploaded on Docker hub.
* <div align="justify">Now once we have this process automated we are going to integrate monitoring using Prometheus and Grafana, this Prometheus and Grafana is going to monitor our EC2 instance as well as Jenkins to check different things in Jenkins like how much is CPU how much is RAM what are some successful jobs what do failed jobs along with this any of the job is failed or success you're also going to get notifications on our email using SMTP.</div>
* And once we automate this, we are going to deploy the application on kubernetes using Argo CD and we will have monitoring (Prometheus and Grafana) on our kubernetes cluster which is going to be installed through HELM charts. 
* Once we do this, we are going to have an application like Netflix.
   
![Alt text](https://github.com/JavierRamirezMoral/DevSecOps-Project-Netflix/blob/main/DOCUMENTACI%C3%93N/DESIGN%20.png)


## Objectives
_DEV PART:_
* Establish a development environment for the application.
* Enable version control and collaboration through GitHub.

_SEC PART:_
* Enhance the security posture of the application.
* Identify and mitigate vulnerabilities in the application's dependencies.

_OPS PART:_
* Ensure consistency and reliability in building and deploying Docker images.
* Facilitate sharing and distribution of Docker images via Docker Hub.
* Ensure high availability and performance of the infrastructure.
* Provide visibility into resource utilization and application health.
* Enable timely response to issues through email notifications.
* Leverage container orchestration for scalability and reliability.
* Automate deployment and management of application resources on Kubernetes.
* Monitor Kubernetes cluster health and performance.
* Build a scalable, resilient, and feature-rich application platform.
* Provide an engaging user experience with seamless content delivery and management

## Brief Summary
<div align="justify">In conclusion, our project has undergone a comprehensive journey towards enhancing security, automation, and monitoring for our application deployment process. We initiated by deploying our application locally on an EC2 instance using Docker containers, followed by integrating security measures via SonarQube and Trivy. This manual setup served as the foundation for automating the process through Jenkins, facilitating the creation of secure Docker images automatically uploaded to Docker Hub.</div> <br>

<div align="justify">Building upon this automation, we integrated monitoring into our deployment pipeline using Prometheus and Grafana, enabling real-time tracking of EC2 instance and Jenkins performance metrics. Notifications via email were implemented to alert stakeholders about job statuses. Subsequently, we extended our automation efforts to Kubernetes deployment utilizing Argo CD, accompanied by the installation of monitoring tools Prometheus and Grafana through HELM charts.</div> <br>


<div align="justify">Through this iterative process, we've transformed our application deployment environment into  a robust, secure, and efficiently managed ecosystem. With the addition of monitoring capabilities, we gain invaluable insights into system health and performance, ensuring proactive identification and resolution of any issues. Ultimately, our project culminates in an application infrastructure resembling that of Netflix, equipped with modern deployment practices and robust monitoring solutions to support its continuous evolution and operation.</div> <br>

