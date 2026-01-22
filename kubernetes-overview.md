# Kubernetes Components Overview

## Helm Package Manager
Helm is a package manager for Kubernetes applications that has evolved from Helm 2 to Helm 3. The main architectural change was moving from a client-server model to a client-only architecture, simplifying deployment and security.

## Autoscaling Types
Kubernetes offers three main types of autoscaling:

1. **Horizontal Pod Autoscaler (HPA)**
   - Adjusts number of pod replicas
   - Based on CPU utilization or custom metrics
   - Works with ReplicaSets, Deployments, and StatefulSets

2. **Vertical Pod Autoscaler (VPA)**
   - Adjusts resource requests and limits for containers
   - Manages CPU and memory allocation
   - Works at the container level

3. **Cluster Autoscaler (CA)**
   - Manages node count in the cluster
   - Automatically adds/removes nodes based on resource needs
   - Handles pod scheduling requirements

## Environment Management
Helm Charts can manage different environments (Development, Staging, Production) using:
- Value files for environment-specific configurations
- Templates for consistent deployment across environments
- Single source of truth with environment-specific parameters
