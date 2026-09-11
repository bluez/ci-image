# bluez/ci-image

Docker image for BlueZ build: ``ghcr.io/bluez/ci-image:latest``

Automatically published to GitHub container registry via push on
main branch.

## Manual build

Docker image can be built manually for internal testing:

```bash
docker build . --file Dockerfile --tag bluez-build:<tag>
```

and can be used to test like

```bash
docker run -ti --workdir /github/workspace -v "<local/path>":"/github/workspace" bluez-build:<tag> /bin/bash
```

## Useful commands

### Pull the image from Github container registry

```bash
docker pull ghcr.io/bluez/ci-image:latest
```

### Show list of images

```bash
docker images
```
