kubectl - 

kubectl apply -f ./deployments.yaml
kubectl get deployments.apps
kubectl get pods

kubectl get replicasets.apps

# name space management
kubectx
kubens

# port forwarding
kubectl port-forward services/nginx 8080:80

kubernetes package manager "helm"

brew install helm 