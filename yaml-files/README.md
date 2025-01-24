# YAML documentation

## nginx-deployment.yaml
This is a **Kubernetes** deployment configuration for an Nginx server. It includes:
- Deployment
- ServiceAccount
- ClusterRole
- ClusterRoleBinding
- PersistentVolumeClaim
- HorizontalPodAutoscaler.

The Deployment specifies the number of replicas, labels, template, service account, volumes, and containers for the Nginx server. The container uses the latest Nginx image and exposes **port 80**. It also includes readiness and liveness probes for health checks.

The ServiceAccount is used for authentication and authorization. The ClusterRole and ClusterRoleBinding define the permissions for the Nginx server. The PersistentVolumeClaim creates a storage request of 1Gi for the Nginx server. The HorizontalPodAutoscaler sets the minimum and maximum number of replicas based on CPU utilization.

## nginx-service.yaml
This is a Kubernetes service definition file for an Nginx server. It defines a service named "nginx-service" that selects pods with the label "app: nginx" and exposes them on port 80. The service type is set to "LoadBalancer" and the load balancer IP is set to 192.168.1.100.