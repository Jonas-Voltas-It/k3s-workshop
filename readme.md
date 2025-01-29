multipass setup


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

get argo cd default admin password
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

kubectl edit applications root-app -n argocd

multipass vm ip address:
192.168.64.2

ingress ip
    - appProtocol: http
      name: http
      nodePort: 30171
      port: 80
      protocol: TCP
      targetPort: http
    - appProtocol: https
      name: https
      nodePort: 30654
      port: 443
      protocol: TCP
      targetPort: https

// check logs
kubectl logs [pod name]


// reinstall argocd
kubectl delete -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml


curl -H "Host: nginx.local" http://192.168.64.2:30171

prisidėti host 

sudo vim /etc/hosts

```
192.168.64.2    nginx.local
```

TODO: next
# secrets => secrets manager
    # external-secrets tool'sas
    # dopler
# domain setup
# metallb - (non http => services tcp/udp ports )
# pihole - add blockeris


gitops repository

