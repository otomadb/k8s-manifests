## Memo

```bash
# Add sealed secret
kubectl apply -f https://github.com/bitnami-labs/sealed-secrets/releases/download/v0.19.4/controller.yaml

kubeseal -o yaml < ./manifest/neo4j-auth.raw.yml > ./manifest/neo4j-auth.yml
kubeseal -o yaml < ./manifest/postgres-auth.raw.yml > ./manifest/postgres-auth.yml
```
