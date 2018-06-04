---
draft: false
weight: 1740
---

## Deploy
```bash
kubectl create -f https://gist.githubusercontent.com/mateimicu/a9ddb794bf0cc62442d19eee3c2fd86c/raw/df7aa7a18b7a41c8ffa62c0e9754bc79414132eb/06_sercret_pod.yml
kubectl create -f https://gist.githubusercontent.com/mateimicu/e192589968d4876a6192712bc07e1bc5/raw/4514eedddeffc498cb0c09d1f9a3fadabf4da5b7/07_secret_service.yml
minikube service service-secret
```
