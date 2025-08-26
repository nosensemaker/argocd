1. Install Argo
$ kubectl create namespace argocd
$ kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

2. Service & Ingress
$ kubectl get svc -n argocd


openssl req -x509 -nodes -days 365 -newkey rsa:2048 \
  -out tls.crt \
  -keyout tls.key \
  -subj "/CN=meu-dominio.com/O=meu-dominio.com"


kubectl create secret tls meu-tls-secret \
  --cert=./tls.crt \
  --key=./tls.key \
  -n <NAMESPACE>



  kubectl get secret argocd-initial-admin-secret -n argocd -o yaml

  echo chave | base64 --decode > argo.txt

  
