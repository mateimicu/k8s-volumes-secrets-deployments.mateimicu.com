---
draft: false
weight: 1620
---
### Deploy
```bash
kubectl create -f https://gist.githubusercontent.com/mateimicu/d8ab1f30f34c1dd14f2256b2604f7688/raw/da34cb2604eaefd79bc610bb9f51d96da2facfcb/10_pod_env_vars.yml
kubectl create -f https://gist.githubusercontent.com/mateimicu/d4902c5a89d5742a12fe2809fdad8c09/raw/83d9b555d36fe19592546399a646be0e960d3b6b/11_configmap_env_service.yml
```

```bash
kubectl exec -ti configmap-env-pod /bin/bash
echo "$SPECIAL_LEVEL_KEY"
```
