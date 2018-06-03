---
draft: false
weight: 2040
---
### Bad Deployment

```bash
kubectl set image deployment/hello-world frontend=bad/bad:bad
kubectl rollout status deployment hello-world
```

```bash
kubectl get rs
```

```bash
kubectl get pods
```
