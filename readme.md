# k8s-argocd

## k8s setup

DockerDesktop Ingress
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v0.46.0/deploy/static/provider/cloud/deploy.yaml


## ArgoCD
https://argoproj.github.io/argo-cd/getting_started/

kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml


kubectl delete -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml


https://argoproj.github.io/argo-cd/getting_started/

GSGXMVtSewjzcVbX
https://github.com/argoproj/argo-workflows




kubectl create ns argo
kubectl apply -n argo -f https://raw.githubusercontent.com/argoproj/argo-workflows/stable/manifests/quick-start-postgres.yaml
kubectl -n argo port-forward deployment/argo-server 2746:2746


https://localhost:2746/workflows/argo

https://github.com/argoproj/argo-events/blob/stable/examples/sensors/webhook.yaml

https://argoproj.github.io/argo-workflows/webhooks/

https://argoproj.github.io/argo-workflows/access-token/