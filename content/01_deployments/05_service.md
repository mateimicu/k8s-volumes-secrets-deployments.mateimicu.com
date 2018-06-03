---
draft: false
weight: 2060
---
### Add a service over our 

{{< gist mateimicu 1c7191ae666ca7aed7656f59e61d0937 >}}
```
kubectl create -f https://gist.githubusercontent.com/mateimicu/1c7191ae666ca7aed7656f59e61d0937/raw/bfc14eab460bfd450150a6e2a4826016b1a7aff5/02_service.yml
kubectl get service service-hello-world
kubectl describe service service-hello-world
minikube service service-hello-world
```
