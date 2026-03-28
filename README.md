# Kubernetes Nginx Deployment

## Overview
This project demonstrates deployment of an Nginx application on Kubernetes using Deployment and Service.

## What I did
- Created Kubernetes cluster using kind
- Deployed nginx using Deployment YAML
- Exposed application using NodePort Service
- Debugged real-world issues:
  - Disk space issues
  - ImagePullBackOff
  - Kubernetes networking issues
- Accessed application via port-forward

## Commands Used

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl get pods
kubectl get svc
kubectl port-forward service/nginx-service 8080:80
