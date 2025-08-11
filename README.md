# Kubernetes Minikube Nginx Deployment

This project demonstrates how to set up a local Kubernetes cluster using **Minikube**, deploy an **Nginx** web server, and verify the deployment.

---

## 📦 Prerequisites

- **Minikube** installed  
- **kubectl** installed  
- A working terminal

---

## 🚀 Steps

### 1. Check Minikube Version
```bash
minikube version
minikube start
kubectl version --client
kubectl create deployment nginx-deployment --image=nginx
kubectl get deployments
kubectl get pods
kubectl describe pod <pod-name>
kubectl expose deployment nginx-deployment --type=NodePort --port=80
minikube service nginx-deployment
minikube stop


📜 Summary
You have successfully:

Started a Minikube cluster

Deployed Nginx

Exposed it to the browser

Verified the service is working

Stopped the cluster
