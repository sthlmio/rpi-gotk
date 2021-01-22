# Flux V2

## Bootstrap/upgrade (idempotent)

```bash
flux bootstrap github \
  --owner=sthlmio \
  --repository=rpi-gotk \
  --branch=main \
  --path=/ \
  --components-extra=image-reflector-controller,image-automation-controller
```

## Monitoring

http://localhost:3000/d/gitops-toolkit-control-plane
http://localhost:3000/d/gitops-toolkit-cluster

```bash
kubectl -n flux-system port-forward svc/grafana 3000:3000
```
