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

http://localhost:3000/d/gitops-toolkit-control-plane

http://localhost:3000/d/gitops-toolkit-cluster

```bash
kubectl -n flux-system port-forward svc/grafana 3000:3000
```
