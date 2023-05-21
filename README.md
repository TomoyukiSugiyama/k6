# k6

xk6-output-influxdb

```bash
K6_INFLUXDB_ORGANIZATION=<insert-here-org-name> \
K6_INFLUXDB_BUCKET=<insert-here-bucket-name> \
K6_INFLUXDB_TOKEN=<insert-here-valid-token> \
~/go/bin/k6 run -o xk6-influxdb=http://localhost:8086 test.js 
```

```bash
kubectl create configmap crocodile-stress-test --from-file test/test.js
kubectl apply -f test/test-cr.yaml
```

## delete

```bash
kubectl delete -f test/test-cr.yaml
```