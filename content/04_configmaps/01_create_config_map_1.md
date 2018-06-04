---
draft: false
weight: 1690
---
### Manual creation
```bash
kubectl create configmap manual-config --from-literal=manual.manual_1=manual_val_1 --from-literal=manual.manual_2=manual_val_2
```

```bash
kubectl get configmap
kubectl describe configmap manual-config
kubectl get configmaps manual-config -o yaml
```

