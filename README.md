# oyd-exercise-2-1

Kubernetes manifests for a small Node.js web application that reads three environment variables (`APP_ENV`, `APP_NAME`, `LOG_LEVEL`) from a ConfigMap and displays them in the browser.

## Evidence

![K8s run](evidence/k8s-run.png)

## Validate and apply

```bash
kubectl apply -f k8s/ --dry-run=client
kubectl apply -f k8s/
kubectl get pods -n webapp
```
