---
layout: post
title: "Devops Project CI/CD With Jenkins, Ansible, Docker, K8s"
categories: [programming, docker, devops, jenkins, ansible, k8s, cicd]
date: 2021-06-05T13:52:36-05:00
draft: false
---

## The course

The course is below.

<https://udemy.com/course/valaxy-devops/>

## My work

My work on this course can be found at the following links:

- <https://github.com/HenryFBP/valaxydevopsproject>
- <https://github.com/HenryFBP/valaxydevopsproject-hello-world-app>

Forked from respectively:

- <https://github.com/yankils/Simple-DevOps-Project>
- <https://github.com/yankils/hello-world>

## Section 1: Introduction

### 1. Introduction

We'll use Git for SCM, Jenkins for CICD pipelines, Maven as build tool, Ansible for configuraton mgmt post-deployment, Docker to host aps, k8s to manage our docker containers.

We'll use AWS to set all of this up.

## DevOps Flow

Devs usually push code to Git.

When code is in Git, Jenkins pulls code and builds.

Once a build is completed, an artifact is generated. This artifact gets deployed to a target environment, which could be a VM, container, or k8s cluster.

We should have a tool that deploys this artifact onto our target environment -- In our case, this is what Ansible does, as a deployment service that deploys on a Docker container or k8s cluster.

![](/images/2021-06-05-devops-project-cicd-with-jenkins-ansible-docker-k8s/devops-flow.png)

### 2. What do we cover

- Intro
    - Intro to CI/CD
    - Tools used to set up DevOps flow

- Setup CI/CD with Jenkins, git, Maven, and Tomcat
    - Set up Jenkins
    - Run a test job
    - Set up and configure Maven + Git
    - Set up Tomcat server
    - Install plugins
    - Integrate Git+Maven in Jenkins
    - Run CI/CD job

- Introducing Docker
    - Set up a docker env
    - Manage Docker with Ansible
    - Docker Hub repo
    - Write Dockerfile
    - Run a job

- Integration with Ansible
    - Set up Ansible env
    - Integrate Ansible with Jenkins
    - Write an Ansible playbook to deploy on a container
    - Running Jobs

- Introducing k8s
    - Set up Kubernetes environment
    - Write deployment and service files
    - Run a job

### 3. What is CI and CD

- CI = Continuous Integration
- CD = Continuous Delivery
- CD = Continuous Deployment

![](/images/2021-06-05-devops-project-cicd-with-jenkins-ansible-docker-k8s/ci.png)

Devs commit, push the commits, then builds/unit tests run, then an artifact is deployed (staging) onto a target environment.

The difference between continuous delivery, and continuous deployment, is that the deploy is /automatic/ for continuous deployment, where in continuous delivery, the deploy step is manual.

And for CI, we just run tests against pushed code, but don't make an artifact.

### 4. Resources to Setup Simple CI/CD Pipeline

1. Github account
    a. `valaxydevopsproject-hello-world-app` repository (see above)
    b. `valaxydevopsproject` repository (see above)
2. AWS Free Tier account.

### 5. Resources before starting

## Section 2: CI/CD pipeline using Git, Jenkins and Maven

### 6. Jenkins Installation

### 7. Run Frist Jenkins Job

### 8. Git Setup

### 9. Correct Git path

### 10. Maven Setup

### 11. Create first Maven job


## Section 3: Integrating Tomcat server in CI/CD pipeline

### 12. Tomcat Server setup

### 13. Deploy a war file on Tomcat VM using
Jenkins

### 14. Common issues: Fork repository

### 15. Deploy on VM through PollSCM

## Section 4: Integrating Docker in CI/CD pipeline

### 16. Docker Setup

### 17. Common issues: Addressing latest tomcat Docker image issue

### 18. Integrating DockerHost with Jenkins

### 19. Jenkins Job to copy artifacts on to DockerHost

### 20. Create a Dockerfile

### 21. Deploy a war file on Docker container using Jenkins

### 22. Troubleshooting: Unable to push docker image

## Section 5: Integrating Ansible in CI/CD pipeline

### 23. Ansible setup

### 24. Troubleshooting: Unable to install Ansible

### 25. Integrate Ansible with Jenkins

### 26. Creating an Ansible playbook

### 27. Common issues faced during practice

### 28. Run Ansible playbooks from Jenkins

### 29. Update Ansible Playbooks to delete and create docker containers

### 30. DockerHub Integration with Ansible

### 31. Tagging Docker image using Ansible playbooks

### 32. Jenkins job to deploy on Docker container through Dockerhub

### 33. Jenkins job to deploy a war file on Docker container using Ansible

## Section 6: Integrating Kubernetes in CI/CD pipeline

### 34. Introduction to Kubernetes Section

### 35. Troubleshooting: panic: runtime error: invalid memory address or nil pointer

### 36. Setup Kubernetes Part-1: Setup Ubuntu Server

### 37. Setup Kubernetes Part-2: Setup Cluster on AWS

### 38. Common Issues: Unable to Access Kubernetes cluster

### 39. Common Issues: Modify K8S Instance sizes & Delete Kubernetes cluster

### 40. Create deployment and service using kubectl commands

### 41. Create deployment and service using YAML files

### 42. Integrate Kubernetes with Ansible

### 43. Create deployment and service using Ansible

### 44. Jenkins CD job to deploy on Kubernetes

### 45. Jenkins CI job to create an Docker image

### 46. Integrating Jenknis CI/CD jobs to deploy on Kubernetes

### 47. Automate deployment on Kubernetes with CI/CD Job

### 48. Setup CI/CD Job for Kubernetes - Final Lab

### 49. Conclusion

## Section 7: Bonus Section

### 50. Bonus Lecture

