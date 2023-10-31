kubectl apply -f deployment.yaml
kubectl expose deployment smartminds-frontend --type=LoadBalancer --name=smartminds-frontend-service
kubectl get services smartminds-frontend-service
