# Kubernetes-Example

## Commands

```bash

# See nodes
kubectl get nodes

# See pods
kubectl get pod

# See services
kubectl get services

# Create deployment
kubectl create deployment nginx-depl --image=nginx

kubectl get deployment

# See logs
kubectl logs  nginx-depl-5c8bf76b5b-ncsht

kubectl create deployment mongo-depl --image=mongo

kubectl logs mongo-depl-5fd6b7d4b4-mznhf

# Access to container
kubectl exec -it mongo-depl-5fd6b7d4b4-mznhf -- bin/bash

# Execute a config file for deployment
kubectl apply -f nginx-deployment.yaml

# Create a secret
kubectl apply -f mongo-secret.yaml

kubectl get secret

# Create service

kubectl get service

kubectl describe service mongodb-service

kubectl get pod -o wide

```
