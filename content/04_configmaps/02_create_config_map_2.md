---
draft: false
weight: 1680
---
### From files
```bash
TEMP=$(mktemp -d)

echo "file_1a=file_val_1" >> "$TEMP/conf1"
echo "file_1b=file_val_2" >> "$TEMP/conf1"

echo "file_2a=file_val_1" >> "$TEMP/conf2"
echo "file_2b=file_val_2" >> "$TEMP/conf2"

ls "$TEMP"
cat "$TEMP/conf1"
cat "$TEMP/conf2"
```

```bash
kubectl create configmap file-config --from-file="$TEMP"
```

```bash
kubectl get configmap
kubectl describe configmap file-config
kubectl get configmaps file-config -o yaml
```
