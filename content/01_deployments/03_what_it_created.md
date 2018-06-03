---
draft: false
weight: 2080
---
### What it did ?

```
kubectl get rs
REPLICA_SET=$(kubectl get rs | grep hello-world | awk '{print $1}')
kubectl describe rs "$REPLICA_SET"
```
