# AI Watsonx and GitHub Sandbox

Welcome to the AI Watsonx and GitHub Sandbox repository! This repository provides YAML files and hands-on demo instructions to practice using **Watsonx Code Assistant** and **GitHub workflows**.

---

## Table of Contents

- [Repository Contents](#repository-contents)
- [Getting Started](#getting-started)
  - [Step 1: Fork the Repository](#step-1-fork-the-repository)
  - [Step 2: Clone Your Fork Locally](#step-2-clone-your-fork-locally)
  - [Step 3: Create a New Branch](#step-3-create-a-new-branch)
- [Contribution Guidelines](#contribution-guidelines)
- [License](#license)

---

## Repository Contents

### YAML Files (Located in `yaml-files/`)

- **`nginx-deployment.yaml`**  
  Defines a Kubernetes Deployment for running an NGINX application with:
  - 3 replicas of the NGINX pod.
  - Resource limits for CPU and memory.
  - Liveness and readiness probes.

- **`nginx-service.yaml`**  
  Defines a Kubernetes Service for exposing the NGINX Deployment with:
  - LoadBalancer type for external access.
  - Target port: 80.

### Demo Instructions (Located in `demo-instructions/`)

- **`exercises.md`**  
  Step-by-step instructions for completing Watsonx and GitHub-related exercises.

---

## Getting Started

### Prerequisites

- GitHub
- Watsonx Code Assistant
- Visual Studio Code (or any other code editor)

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

## Contribution Guidelines

We welcome contributions! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch for your changes.
3. Make your changes and commit them with clear and concise messages.
4. Push your changes to your fork.
5. Create a pull request to the `main` branch of this repository.

For detailed guidelines, please refer to our [CONTRIBUTING.md](CONTRIBUTING.md) file.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Happy learning and collaborating!

---
