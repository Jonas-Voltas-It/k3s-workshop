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

get admin password
kubectl get secrets argocd-initial-admin-secret -oyaml
echo eFFSTGtSMEs3VThDWWYydA== |base64 -d
xQRLkR0K7U8CYf2t

kubectl port-forward svc/argocd-server 8080:80


app of apps argo cd

delete commands
kubectl delete deployment nginx-deployment -n default
kubectl delete pod nginx -n default
kubectl delete service nginx -n default


brew install kustomize