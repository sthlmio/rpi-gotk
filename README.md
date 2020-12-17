# Flux V2

## Bootstrap (idempotent)

```bash
flux bootstrap github \
  --owner=sthlmio \
  --repository=rpi-gotk \
  --branch=main \
  --arch=arm64 \
  --components-extra=image-reflector-controller,image-automation-controller
```
