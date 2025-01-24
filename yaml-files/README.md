nginx-deployment.yaml

This is an example of a YAML file for deploying Nginx on Kubernetes. The file defines a deployment with three replicas, a selector to match the app label, and a template for the pod spec. The pod spec includes a container for Nginx, with the latest image, port 80, CPU and memory limits, and liveness and readiness probes.

To add documentation to this code, you can use comments in the YAML file to explain the purpose and functionality of each section. For example:


// Assisted by watsonx Code Assistant 
# nginx-deployment.yaml

# Deployment configuration
spec:
  # Number of replicas
  replicas: 3
  # Selector to match pods
  selector:
    matchLabels:
      app: nginx
  # Pod template
  template:
    # Metadata for the pod
    metadata:
      labels:
        app: nginx
    # Pod spec
    spec:
      # Container for Nginx
      containers:
      - name: nginx
        # Image for Nginx
        image: nginx:latest
        # Port to expose
        ports:
        - containerPort: 80
        # Resource limits
        resources:
          limits:
            cpu: "500m"
            memory: "1Gi"
        # Liveness probe
        livenessProbe:
          # Path to check
          httpGet:
            path: /
            # Port to check
            port: 80
          # Initial delay and period
          initialDelaySeconds: 5
          periodSeconds: 5
        # Readiness probe
        readinessProbe:
          # Path to check
          httpGet:
            path: /
            # Port to check
            port: 80
          # Initial delay and period
          initialDelaySeconds: 5
          periodSeconds: 5
This documentation provides information about the deployment configuration, pod template, container, and probes. It explains the purpose and functionality of each section, including the parameters and return types.


nginx-service.yaml

This YAML file defines a Kubernetes Service named `nginx-service` that exposes port 80 of the `nginx` application. The service uses the `LoadBalancer` type, which means it will be exposed externally via a cloud load balancer.

The `selector` field specifies the labels that the `nginx` pods must have in order to be selected by the service. In this case, the `app` label must be set to `nginx`.

The `ports` field specifies the port that the service will expose internally and the port that the target pods will receive. In this case, port 80 of the service will forward to port 80 of the target pods.

Overall, this YAML file defines a basic Kubernetes Service that exposes the `nginx` application externally via a cloud load balancer.
