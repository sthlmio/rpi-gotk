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
