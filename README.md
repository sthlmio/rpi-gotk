# Flux V2

Current version: `0.5.3`

## Bootstrap (idempotent)

```bash
flux bootstrap github \
  --owner=sthlmio \
  --repository=rpi-gotk \
  --branch=main \
  --arch=arm64 \
  --components-extra=image-reflector-controller,image-automation-controller
```
