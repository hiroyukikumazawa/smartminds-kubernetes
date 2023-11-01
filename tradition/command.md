kubectl apply -f deployment.yaml
kubectl expose deployment smartminds-frontend --type=NodePort --name=smartminds-frontend-service
kubectl get services smartminds-frontend-service
