## Deps

Cert-Manager:
```bash
  kubectl apply --validate=false -f https://github.com/jetstack/cert-manager/releases/download/v1.1.0/cert-manager.yaml
```

```yaml
spec:
  routes:
  - services:
    - name: rootapp
      port: 80
    conditions:
    - prefix: /
    authPolicy:
      disabled: true
```

```bash
curl -i -k --user user1:password1 https://local.projectcontour.io
```