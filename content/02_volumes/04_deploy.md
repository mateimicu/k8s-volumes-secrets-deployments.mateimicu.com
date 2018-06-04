---
draft: false
weight: 1960
---

## Deploy
```bash
kubectl create -f https://gist.githubusercontent.com/mateimicu/273ffee7d9e1cb9d4a1a45cfed037a97/raw/f93c74f9e96519fafa953a44f37ea6cd0f0a8dfe/03_empty_dir.yml
kubectl create -f https://gist.githubusercontent.com/mateimicu/463c2706fe7404a18bc2343da90dbad1/raw/04561abc4597733376d16b4d429d5e50167bae85/04_empty_dir_service.yml
minikube service service-emptydir-volume
```
