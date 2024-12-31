# Demo Exercises for AI Watsonx and GitHub

Follow these exercises to learn how to use Watsonx Code Assistant and GitHub workflows effectively.

---

## Exercise 1: Explain YAML Files

1. Open `yaml-files/nginx-deployment.yaml` in Visual Studio Code.
2. Use Watsonx Code Assistant to explain the file:
   ```bash
   /explain @nginx-deployment.yaml
   ```
3. Repeat for `nginx-service.yaml`:
   ```bash
   /explain @nginx-service.yaml
   ```

## Exercise 2: Generate Documentation
1. Use Watsonx Code Assistant to generate documentation for each YAML file:
   ```bash
   /document @nginx-deployment.yaml
   /document @nginx-service.yaml
   ```
2. Save the output as `README.md` in the `yaml-files/` directory.

## Exercise 3: Enhance the YAML Files
1. Add resource limits to `nginx-deployment.yaml` using Watsonx:
   ```bash
   Add resource limits for CPU and memory to @nginx-deployment.yaml
   ```
2. Add liveness and readiness probes to the containers:
   ```bash
   Add liveness and readiness probes to @nginx-deployment.yaml
   ```

## Exercise 4: Collaborative Workflow with GitHub
1. Commit and push your changes to your forked repository:
   ```bash
   git add .
   git commit -m "Enhance YAML files with resource limits and probes"
   git push origin main
   ```
2. Create a Pull Request to this repository:
   - Go to your forked repository on GitHub.
   - Click on the **Pull Requests** tab.
   - Click the **New Pull Request** button.
   - Select the base repository and branch to merge your changes.
   - Title: Enhance YAML files with resource limits and probes.
   - Description: Briefly describe your changes.
   - Click **Create Pull Request**.
3. Review and comment on each other’s Pull Requests.
4. Create an issue to suggest further enhancements, such as adding a Node.js deployment YAML.

Happy learning!

---