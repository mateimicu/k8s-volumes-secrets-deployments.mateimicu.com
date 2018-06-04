---
draft: false
weight: 1720
---
```
apiVersion: v1
kind: Pod
metadata:
  name: test-secret
  labels:
      type: python-fend2
spec:
  containers:
  - image: matei10/hello-mambu-local-storage:0.0.8
    name: python-fend2
    env:
      - name: SECRET_PASSWORD
        valueFrom:
          secretKeyRef:
            name: mambu-secret
            key: password
```
