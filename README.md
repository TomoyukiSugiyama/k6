# k6

```bash
k6 run test.js
```

```bash
kubectl create configmap crocodile-stress-test --from-file test/test.js
kubectl apply -f test/test-cr.yaml
```

## delete

```bash
kubectl delete -f test/test-cr.yaml
```