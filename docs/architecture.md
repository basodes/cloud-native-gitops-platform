# Cloud Native GitOps Platform Architecture

```mermaid
flowchart TD

A[Developer] -->|Git Push| B[GitHub Repository]

B --> C[GitHub Actions CI/CD]

C -->|Build Docker Image| D[Docker Hub]

B -->|Kubernetes Manifests| E[ArgoCD]

D --> E

E -->|Sync| F[Kubernetes Cluster]

F --> G[Frontend Pods]

F --> H[Backend Pods]

F --> I[Prometheus]

I --> J[Grafana]
```

## Workflow

1. Developer pushes code to GitHub.
2. GitHub Actions builds Docker images.
3. Images are pushed to Docker Hub.
4. ArgoCD monitors GitHub repository.
5. ArgoCD syncs changes to Kubernetes.
6. Kubernetes deploys new application version.
7. Prometheus collects metrics.
8. Grafana visualizes cluster health.