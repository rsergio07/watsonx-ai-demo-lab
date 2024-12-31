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

*Why?*  
Forking allows you to create your own copy of this repository so you can safely make changes without affecting the original.

---

### Step 2: Clone Your Fork Locally
1. Clone your forked repository:
   ```bash
   git clone https://github.com/<your-username>/ai-watsonx-github.git
   cd ai-watsonx-github
   ```

*Why?*  
Cloning downloads the repository to your local machine, so you can work on it using your favorite tools like Visual Studio Code.

---

### Step 3: Create a New Branch
1. Create and switch to a new branch:
   ```bash
   git checkout -b my-enhancements
   ```

*Why?*  
Working on a new branch helps keep your changes isolated from the main branch. This makes it easier to manage and collaborate on different tasks.

---

### Step 4: Make and Commit Your Changes
1. Check the status of your changes:
   ```bash
   git status
   ```

2. Stage all your changes:
   ```bash
   git add .
   ```

3. Confirm the staged changes:
   ```bash
   git status
   ```

4. Commit your changes with a descriptive message:
   ```bash
   git commit -m "Add liveness and readiness probes to nginx-deployment.yaml"
   ```

5. Push your branch to your fork:
   ```bash
   git push origin my-enhancements
   ```

Happy learning and collaborating!

---