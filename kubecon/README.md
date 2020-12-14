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
curl -i https://stevesloka.dev/secure
curl -i --user user1:password1 https://stevesloka.dev/secure
```