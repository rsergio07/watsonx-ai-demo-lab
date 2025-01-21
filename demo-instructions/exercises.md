# Demo Exercises for AI Watsonx and GitHub

Follow these exercises to learn how to use Watsonx Code Assistant and GitHub workflows effectively.

---

## Exercise 1: Explain YAML Files
**Objective**: Understand the structure and purpose of YAML files using Watsonx Code Assistant.

1. Open `yaml-files/nginx-deployment.yaml` in Visual Studio Code.
2. Use Watsonx Code Assistant to explain the file:
    ```bash
    /explain @nginx-deployment.yaml
    ```
3. Repeat for `nginx-service.yaml`:
    ```bash
    /explain @nginx-service.yaml
    ```

---

## Exercise 2: Enhance the YAML Files
**Objective**: Improve the YAML files by adding resource limits and probes.

1. Add resource limits to `nginx-deployment.yaml` using Watsonx:
    ```bash
    Add resource limits for CPU and memory to @nginx-deployment.yaml
    ```
2. Add liveness and readiness probes to the containers:
    ```bash
    Add liveness and readiness probes to @nginx-deployment.yaml
    ```

**Note**: Make sure to update your local `nginx-deployment.yaml` file with the code suggested by Watsonx Code Assistant. This step ensures that the file contains the latest enhancements, so the next steps will be based on the updated file.

---

## Exercise 3: Generate Documentation
**Objective**: Generate professional-grade documentation for YAML files with Watsonx Code Assistant.

1. Use Watsonx Code Assistant to generate documentation for each YAML file:
    ```bash
    /document @nginx-deployment.yaml
    ```
2. Repeat for `nginx-service.yaml`:
    ```bash
    /document @nginx-service.yaml
    ```
3. Save the output as `README.md` in the `yaml-files/` directory.

---

## Exercise 4: Make and Commit Your Changes
**Objective**: Practice using Git commands to track and push changes to GitHub.

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
    git commit -m "Enhance nginx-deployment.yaml with resource limits and probes, and generate documentation"
    ```
5. Push your branch to your fork:
    ```bash
    git push origin my-enhancements
    ```

---

## Exercise 5: Collaborate with Pull Requests and Issues

---

### **Step 1: Create a Pull Request (PR)**
**Objective**: Propose your changes for review by submitting a Pull Request to the original repository.

1. Navigate to your forked repository on GitHub.
2. Click on the **Pull Requests** tab.
3. Click the **New Pull Request** button.
4. In the PR interface:
    - Select the base repository (`rsergio07/ai-watsonx-github`) and branch (e.g., `main`) as the target for your PR.
    - Select the branch with your changes (e.g., `my-enhancements`) as the source branch.
5. Add a clear and descriptive title, such as:
    - *Enhance YAML files with resource limits and probes.*
6. Write a brief but informative description of your changes, highlighting:
    - The modifications you made (e.g., added resource limits, liveness probes).
    - The purpose of the changes and any relevant context.
7. Click **Create Pull Request** to submit your PR.

---

### **Step 2: Review and Comment on Peer Pull Requests**
**Objective**: Foster collaboration by reviewing and providing feedback on Pull Requests submitted by peers.

1. Go to the **Pull Requests** tab in the base repository.
2. Review PRs submitted by other participants:
    - Open a PR and read through the description and code changes.
    - Leave constructive comments, such as:
      - Suggestions for improvement.
      - Questions about specific changes.
      - Positive feedback for well-written code or creative solutions.
3. Mark PRs as "Approved" or suggest changes as needed.

---

### **Step 3: Create a GitHub Issue**
**Objective**: Suggest enhancements or propose new tasks using GitHub Issues.

1. Go to the **Issues** tab in the base repository.
2. Click the **New Issue** button.
3. Create an issue to propose an enhancement. For example:
    - **Title**: Add a Node.js deployment YAML.
    - **Description**:
      - "Propose adding a new YAML file for deploying a simple Node.js application. This can include readiness and liveness probes and resource limits similar to the NGINX example."
4. Assign the issue to yourself or a peer to work on collaboratively.

---

Happy learning and collaborating!

---
