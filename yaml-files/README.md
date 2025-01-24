// Assisted by watsonx Code Assistant 
//nginx-deployment.yaml

//nginx-deployment.yaml
apiVersion: apps/v1 // Kubernetes API version
kind: Deployment // Type of Kubernetes resource
metadata: // Metadata for the deployment
  name: nginx-deployment // Name of the deployment
spec: // Specification for the deployment
  replicas: 3 // Number of replicas for the deployment
  selector: // Selector for the deployment
    matchLabels:
      app: nginx // Match labels for the deployment
  template: // Template for the pod
    metadata: // Metadata for the pod
      labels:
        app: nginx // Labels for the pod
    spec: // Specification for the pod
      containers: // List of containers in the pod
      - name: nginx // Name of the container
        image: nginx:latest // Image for the container
        ports: // List of ports to expose in the container
        - containerPort: 80 // Port to expose in the container
        resources: // Resource limits for the container
          limits:
            cpu: "500m" // CPU limit for the container
            memory: "1Gi" // Memory limit for the container
        livenessProbe: // Liveness probe for the container
          httpGet:
            path: / // Path to use for the probe
            port: 80 // Port to use for the probe
          initialDelaySeconds: 5 // Initial delay for the probe
          periodSeconds: 5 // Period for the probe
        readinessProbe: // Readiness probe for the container
          httpGet:
            path: / // Path to use for the probe
            port: 80 // Port to use for the probe
          initialDelaySeconds: 5 // Initial delay for the probe
          periodSeconds: 5 // Period for the probe


//nginx-service.yaml
This YAML file defines a Kubernetes Service named `nginx-service` that exposes port 80 of the `nginx` application. The service uses the `LoadBalancer` type, which means it will be exposed externally via a cloud load balancer.

The `selector` field specifies the labels that the `nginx` pods must have in order to be selected by the service. In this case, the `app` label must be set to `nginx`.

The `ports` field specifies the port that the service will expose internally and the port that the target pods will receive. In this case, port 80 of the service will forward to port 80 of the target pods.

Overall, this YAML file defines a basic Kubernetes Service that exposes the `nginx` application externally via a cloud load balancer.

