kubectl apply -f nginx-deployment.yaml
kubectl expose deployment nginx-deployment --type=NodePort --name=nginx-service
kubectl apply -f nginx-https-service.yaml
