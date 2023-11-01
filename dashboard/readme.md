## creating service account and get access token
https://github.com/kubernetes/dashboard/blob/master/docs/user/access-control/creating-sample-user.md

## commands
kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.7.0/aio/deploy/recommended.yaml
kubectl apply -f dashboard\dashboard-adminuser.yaml
kubectl -n kubernetes-dashboard create token admin-user
kubectl proxy

## dashboard url
http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/.