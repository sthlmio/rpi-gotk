# rpi-gotk

GitOps repo for Flux v2 running on our Raspberry Pi Kubernetes cluster.

## Bootstrap/upgrade (idempotent)

```bash
brew upgrade fluxcd/tap/flux

flux bootstrap github \
  --owner=sthlmio \
  --repository=rpi-gotk \
  --branch=main \
  --path=/ \
  --components-extra=image-reflector-controller,image-automation-controller
```

## Monitoring

http://127.0.0.1:3000/

```bash
kubectl -n flux-system port-forward svc/grafana 3000:3000
```
