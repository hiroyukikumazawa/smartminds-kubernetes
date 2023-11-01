kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.3.0/deploy/static/provider/cloud/deploy.yaml
kubectl apply -f ingress\deployment.yaml
<!-- kubectl expose deployment smartminds-frontend --type=NodePort --name=smartminds-frontend-service -n ingress-nginx -->
kubectl apply -f ingress\service.yaml
kubectl create secret tls collab-secret --cert=certificate\server.cer --key=certificate\server.key
kubectl apply -f ingress\ingress.yaml
