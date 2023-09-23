## Memo

### Requirements

- [kubernetes/ingress-nginx](https://github.com/kubernetes/ingress-nginx)
- [ArgoCD](https://argo-cd.readthedocs.io)
  - namespace は`argocd`とする．

### Memo

```bash
task prod:apply-projects

task prod:sealed-secrets-backup # 鍵のバックアップ
task prod:encrypt # Secretsの暗号化
```
