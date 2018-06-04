---
draft: false
weight: 1730
---

#### Allow a specific path from a secret
```bash
 volumes:
  - name: second-secret
    secret:
      secretName: mambu-secret2
      items:
      - key: password
        path: new-dir/new-password
```

#### file permisions
decimal notation
```bash
 volumes:
  - name: second-secret
    secret:
      secretName: mambu-secret2
      defaultMode: 511
```
