---
draft: false
weight: 2050
---
### Deploy new version

```
kubectl set image deployment/hello-world frontend=matei10/docker-hello-world:0.0.2
```

### Check status
```
kubectl rollout status deployment hello-world
kubectl get rs
```
