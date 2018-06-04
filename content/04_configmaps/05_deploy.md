---
draft: false
weight: 1650
---
### Deploy
```bash
kubectl create -f https://gist.githubusercontent.com/mateimicu/196396fab94b795d7c94575c4d2bfa1e/raw/467e05f46e9ad898b715abcb43d19d82a2ee7e6f/08_pod_config_map.yml
kubectl create -f https://gist.githubusercontent.com/mateimicu/b4892b0615d14f5c8d2bb1837f13ce17/raw/8589e7e3097ee404388a012fe2956b88713f1dca/09_configmap_service.yml
```

```bash
kubectl exec -ti configmap-file-pod ls /config
kubectl exec -ti configmap-file-pod ls /config
```
