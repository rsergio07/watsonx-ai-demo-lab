// Assisted by watsonx Code Assistant 
//nginx-deployment.yaml
 

// Deployment configuration for a Nginx server
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
spec:
  replicas: 3
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx
        // Container for the Nginx server
        image: nginx:latest
        ports:
        - containerPort: 80
        resources:
          limits:
            cpu: "500m"
            memory: "1Gi"
        livenessProbe:
          // Probe to check the liveness of the container
          httpGet:
            path: /
            port: 80
          initialDelaySeconds: 5
          periodSeconds: 5
        readinessProbe:
          // Probe to check the readiness of the container
          httpGet:
            path: /
            port: 80
          initialDelaySeconds: 5
          periodSeconds: 5



This YAML file defines a Kubernetes Service named `nginx-service` that exposes port 80 of the `nginx` application. The service uses the `LoadBalancer` type, which means it will be exposed externally via a cloud load balancer.

The `selector` field specifies the labels that the `nginx` pods must have in order to be selected by the service. In this case, the `app` label must be set to `nginx`.

The `ports` field specifies the port that the service will expose internally and the port that the target pods will receive. In this case, port 80 of the service will forward to port 80 of the target pods.

Overall, this YAML file defines a basic Kubernetes Service that exposes the `nginx` application externally via a cloud load balancer.
