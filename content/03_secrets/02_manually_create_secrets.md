---
draft: false
weight: 1780
---

```bash
echo -n 'cloudy2010' | base64 # => Y2xvdWR5MjAxMA==
```

{{< gist mateimicu 3b6c174cfb21e87cfbf22e3eb0291ef5 >}}

```bash
kubectl create -f https://gist.githubusercontent.com/mateimicu/3b6c174cfb21e87cfbf22e3eb0291ef5/raw/acdb468a148d67546e4432bb41f8787a06e875aa/05_secret.yml
```

```bash
kubectl get secrets
```

```bash
kubectl describe secrets mambu-secret
```
