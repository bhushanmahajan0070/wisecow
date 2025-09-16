# Wisecow

Cow Wisdom Web Server - A simple web server that serves random cow quotes using fortune and cowsay commands.

![Wisecow Logo](https://raw.githubusercontent.com/nyrahul/wisecow/main/wisecow-logo.png)

---

## Table of Contents

- [About](#about)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Kubernetes Deployment](#kubernetes-deployment)
- [CI/CD Pipeline](#cicd-pipeline)
- [TLS/SSL Support](#tlsssl-support)
- [Scripts for Monitoring](#scripts-for-monitoring)
- [Contributing](#contributing)
- [License](#license)
- [Credits](#credits)
- [Contact](#contact)

---

## About

Wisecow is a lightweight web server built on Debian using `fortune-mod` and `cowsay` to display fun and inspirational cow wisdom messages. It is containerized with Docker and deployable on Kubernetes clusters. This project includes Kubernetes manifests, TLS implementation, and GitHub Actions CI/CD pipelines for fully automated build and deployment.

---

## Features

- Dockerized Wisecow web application
- Kubernetes manifests for deployment and service exposure
- TLS/SSL support for secure communication
- GitHub Actions workflow to automate build, push, and deploy
- Monitoring scripts for system and application health

---

## Prerequisites

Before running the project, ensure you have:

- Docker installed on your machine
- Kubernetes cluster ready (Minikube, Kind, or any cloud provider)
- kubectl CLI configured to interact with your Kubernetes cluster
- GitHub account and Docker Hub (or other container registry) account

---

## Installation

1. Clone the repository:






# Cow wisdom web server

## Prerequisites

```
sudo apt install fortune-mod cowsay -y
```

## How to use?

1. Run `./wisecow.sh`
2. Point the browser to server port (default 4499)

## What to expect?
![wisecow](https://github.com/nyrahul/wisecow/assets/9133227/8d6bfde3-4a5a-480e-8d55-3fef60300d98)

# Problem Statement
Deploy the wisecow application as a k8s app

## Requirement
1. Create Dockerfile for the image and corresponding k8s manifest to deploy in k8s env. The wisecow service should be exposed as k8s service.
2. Github action for creating new image when changes are made to this repo
3. [Challenge goal]: Enable secure TLS communication for the wisecow app.

## Expected Artifacts
1. Github repo containing the app with corresponding dockerfile, k8s manifest, any other artifacts needed.
2. Github repo with corresponding github action.
3. Github repo should be kept private and the access should be enabled for following github IDs: nyrahul
