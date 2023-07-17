# Deployment config for Kubernetes

use with ArgoCD and Helm

## Prerequisite

- Kubernetes (k3s / k8s)
- ArgoCD (https://argo-cd.readthedocs.io/en/stable/getting_started/)

## How to use this repo

Link this repo with ArgoCD (don't forget to create a GitHub access token for authentication)

Add application and enter helm chart values (if they exists)

Create a deployment and wait for ArgoCD to sync.

Enjoy!

## Cli

To see all endpoints in the deployment application

```bash
kubectl get ep --namespace=<your_k8s_namespace>
```

To get all services in the deployment application

```bash
kubectl -n <your_k8s_namespace> get svc
```
