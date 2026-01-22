[README.md](https://github.com/user-attachments/files/24796172/README.md)
# Kubernetes Production-Ready Portfolio

[![Author](https://img.shields.io/badge/Author-bekiryagan-blue?style=for-the-badge)](https://github.com/bekiryagan)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-v1.28+-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)](https://kubernetes.io/)
[![Helm](https://img.shields.io/badge/Helm-v3.12+-0F1689?style=for-the-badge&logo=helm&logoColor=white)](https://helm.sh/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?style=for-the-badge)](http://makeapullrequest.com)

> Enterprise-grade Kubernetes configurations, Helm charts, and deployment patterns for production environments. Built with security, scalability, and observability in mind.

## What's Inside

This repository showcases **real-world Kubernetes expertise** through battle-tested configurations covering:

- **Infrastructure as Code** - Complete RBAC, namespaces, quotas, and network policies
- **Microservices Deployment** - Production-ready FastAPI application with MySQL and Redis
- **Database Clusters** - StatefulSets with replication, backups, and high availability
- **Observability** - Full Prometheus, Grafana, and Alertmanager stack
- **GitOps** - ArgoCD and Flux configurations for continuous deployment
- **Autoscaling** - HPA, VPA, KEDA, and Cluster Autoscaler examples
- **Security** - OPA Gatekeeper, Pod Security Standards, Network Policies
- **Disaster Recovery** - Velero backups and multi-cluster federation

## Repository Structure

```
kubernetes-portfolio/
├── 01-core-infrastructure/     # Namespaces, RBAC, Resource Quotas, Network Policies
├── 02-microservices-app/       # FastAPI deployment with all production requirements
├── 03-database-clusters/       # MySQL and Redis StatefulSets with HA
├── 04-observability-stack/     # Prometheus, Grafana, Alertmanager
├── 05-ci-cd-pipelines/         # ArgoCD GitOps configuration
├── 07-autoscaling/             # HPA, VPA, KEDA advanced scaling
├── 08-security/                # OPA Gatekeeper, Pod Security, Audit Policies
├── 09-helm-charts/             # Production Helm chart for FastAPI
├── 10-gitops/                  # Flux v2 configuration
├── 11-disaster-recovery/       # Velero backups and restore strategies
└── 12-multi-cluster/           # Kubernetes Federation setup
```

## Quick Start

```bash
# Clone the repository
git clone https://github.com/bekiryagan/kubernetes-portfolio.git
cd kubernetes-portfolio

# Apply core infrastructure (namespaces, RBAC, quotas)
kubectl apply -f 01-core-infrastructure/

# Deploy the FastAPI microservice
kubectl apply -f 02-microservices-app/

# Deploy database clusters
kubectl apply -f 03-database-clusters/

# Install observability stack
kubectl apply -f 04-observability-stack/

# Or use Helm for the FastAPI app
helm install fastapi ./09-helm-charts/fastapi-chart -n production
```

## Key Features

| Feature | Description |
|---------|-------------|
| **Security First** | Pod Security Standards, OPA policies, Network Policies, RBAC |
| **Production Ready** | Resource limits, health probes, PDBs, anti-affinity rules |
| **Observable** | Prometheus metrics, Grafana dashboards, alerting rules |
| **Scalable** | HPA, VPA, KEDA for event-driven scaling |
| **GitOps Native** | ArgoCD and Flux configurations included |
| **Multi-Environment** | Dev, staging, production value files |
| **Disaster Recovery** | Velero backup schedules and restore procedures |
| **Multi-Cluster** | Federation and multi-cluster ingress examples |

## Technologies Used

- **Container Orchestration**: Kubernetes 1.28+
- **Package Management**: Helm 3.12+
- **GitOps**: ArgoCD, Flux v2
- **Monitoring**: Prometheus, Grafana, Alertmanager
- **Databases**: MySQL 8.0, Redis 7.2
- **Autoscaling**: HPA, VPA, KEDA
- **Security**: OPA Gatekeeper, Falco, Network Policies
- **Backup**: Velero
- **Service Mesh Ready**: Istio compatible

## Prerequisites

- Kubernetes 1.28+ cluster
- kubectl configured with cluster access
- Helm 3.12+
- (Optional) ArgoCD for GitOps
- (Optional) Metrics Server for HPA
- (Optional) cert-manager for TLS

## Documentation

Each directory contains detailed comments explaining:
- Architecture decisions and trade-offs
- Configuration options and customization
- Security considerations
- Troubleshooting tips

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Author

**Bekir Yagan**

- GitHub: [@bekiryagan](https://github.com/bekiryagan)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

If you find this repository helpful, please give it a star!
