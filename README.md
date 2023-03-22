## Memo

### Requirements

- [kubernetes/ingress-nginx](https://github.com/kubernetes/ingress-nginx)
- [ArgoCD](https://argo-cd.readthedocs.io)
  - namespace は`argocd`とする．

### Apply

```bash
kubectl apply -k ./argocd/prod
```

### Update secrets

```
sops -e ./secrets.yaml > ./secrets.enc.yaml
```
