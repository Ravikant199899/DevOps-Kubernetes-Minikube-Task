Kubernetes Minikube Nginx Deployment
This project demonstrates how to set up a local Kubernetes cluster using Minikube, deploy an Nginx web server, and verify the deployment.

📦 Prerequisites
Minikube installed

kubectl installed

Access to a working terminal

🚀 Step-by-Step Instructions

1. Check Minikube Version

minikube version
minikube-version.png

2. Start Minikube

minikube start
minikube-start.png 

3. Kubectl Version

kubectl version --client
kubectl-version.png

4. Deploy Nginx

kubectl create deployment nginx-deployment --image=nginx

5. View Deployments

kubectl get deployments
kubectl-get-deployments.png

6. View Pods

kubectl get pods
kubectl-get-pods.png

7. Describe Pod

kubectl describe pod <pod-name>
describe-pod-log-pod.png

8. Expose Deployment & Access Nginx

kubectl expose deployment nginx-deployment --type=NodePort --port=80
minikube service nginx-deployment
Nginx-page.png 

9. Stop Minikube
    
bash
minikube stop
Minikube-stop.png


📜 Summary
You have completed the following:

Started a Minikube cluster

Deployed Nginx

Exposed Nginx to the browser

Verified the deployment

Stopped the cluster

💡 README Tips
Use code blocks for commands.

Use screenshots after each major step to visually document your process.

Keep all steps concise for quick reference.
