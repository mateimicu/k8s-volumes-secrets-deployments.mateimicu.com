---
draft: false
weight: 1970
---

####  Where is the volume ?

```bash
kubectl get pod test-emptydir -o json
POD_UUID=$(kubectl get pod -n default test-emptydir -o 'jsonpath={.metadata.uid}')
echo "UUID :$POD_UUID"
minikube ssh
sudo su
cd /var/lib/kubelet/pods/
```

