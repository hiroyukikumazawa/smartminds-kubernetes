kubectl apply -f collablive-deployment.yaml
kubectl expose deployment collablive-deployment --type=NodePort --name=collablive-service
kubectl expose deployment collablive-deployment --type=LoadBalancer --name=collablive-service
kubectl apply -f collablive-https-service.yaml
