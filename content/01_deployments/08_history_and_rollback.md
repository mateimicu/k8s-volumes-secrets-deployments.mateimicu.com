---
draft: false
weight: 2030
---
##### Deployment history

```bash
kubectl rollout history deployment/hello-world
```

#####  CHANGE-CAUSE empty ?
```bash
kubectl set image deployment/hello-world frontend=bad/bad:2bad --record
```

```bash
kubectl rollout history deployment/hello-world
```

```bash
kubectl rollout history deployment/hello-world --revision=1
```

```bash
kubectl rollout undo deployment/hello-world --to-revision=2
```

##### Status
```bash
kubectl rollout status deployment hello-world
```
