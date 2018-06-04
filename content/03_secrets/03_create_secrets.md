---
draft: false
weight: 1770
---

```bash
echo -n 'cloudy2010' > password2
```

```bash
kubectl create secret generic mambu-secret2 --from-file=./password2
```

```bash
kubectl get secrets
```

```bash
kubectl describe secrets mambu-secret2
```
