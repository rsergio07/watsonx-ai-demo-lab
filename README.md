# AI Watsonx and GitHub Sandbox

Welcome to the AI Watsonx and GitHub Sandbox repository! This repository provides YAML files and hands-on demo instructions to practice using **Watsonx Code Assistant** and **GitHub workflows**.

---

## Repository Contents

### YAML Files (Located in `yaml-files/`)
- **`nginx-deployment.yaml`**  
  Defines a Kubernetes Deployment for running an NGINX application with:
  - 3 replicas of the NGINX pod.
  - Resource limits for CPU and memory.

- **`nginx-service.yaml`**  
  Defines a Kubernetes Service for exposing the NGINX Deployment with:
  - LoadBalancer type for external access.
  - Target port: 80.

### Demo Instructions (Located in `demo-instructions/`)
- **`exercises.md`**  
  Step-by-step instructions for completing Watsonx and GitHub-related exercises.

---

## Getting Started

### Step 1: Fork the Repository
1. Click the **Fork** button at the top-right corner of this repository's page.
2. Create a forked copy in your GitHub account.

### Step 2: Clone Your Fork Locally
```bash
git clone https://github.com/<your-username>/ai-watsonx-github.git
cd ai-watsonx-github
