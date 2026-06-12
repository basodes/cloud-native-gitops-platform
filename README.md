# Cloud Native GitOps Platform

## Overview

A cloud-native DevOps platform demonstrating GitOps workflows using Kubernetes, ArgoCD, Terraform, Prometheus, and Grafana.

This project showcases Infrastructure as Code (IaC), Continuous Deployment, Kubernetes orchestration, monitoring, and observability.

---

## Architecture

GitHub Repository
↓
ArgoCD
↓
Kubernetes Cluster
├── Frontend Application
├── Backend Application
├── NGINX Ingress Controller
└── Monitoring Stack
├── Prometheus
└── Grafana

---

## Technologies Used

* Docker
* Kubernetes
* ArgoCD
* Terraform
* GitHub Actions
* Prometheus
* Grafana
* NGINX Ingress
* Helm

---

## Features

* GitOps deployment workflow
* Automated synchronization using ArgoCD
* Kubernetes self-healing
* Infrastructure as Code using Terraform
* Monitoring and observability
* NGINX ingress routing
* Horizontal scaling support

---

## Project Structure

```text
cloud-native-gitops-platform/
├── .github/workflows
├── argocd
├── kubernetes
├── monitoring
├── terraform
├── docs
└── README.md
```

## Demo Commands

```bash
kubectl get pods -n gitops-platform

kubectl get ingress -n gitops-platform

kubectl get applications -n argocd

kubectl get pods -n monitoring
```

## Future Improvements

* AWS EKS deployment
* Terraform remote state
* Horizontal Pod Autoscaler
* Loki log aggregation
* Service Mesh integration
