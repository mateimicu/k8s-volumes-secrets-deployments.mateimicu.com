---
draft: false
weight: 2070
---
### Pod Hash
Used by replica sets
```
kubectl describe rs "$REPLICA_SET"
```
```
kubectl get pods --show-labels=true    
```

#### matchLabels
Used by Deployments to monitor overall status (across multiple replica sets)
