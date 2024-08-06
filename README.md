# nesi-ondemand-base

```
cd packer
packer build base-template.json
packer build vnc-template.json
```

```
docker push ghcr.io/lbrick/nesi-docker-base/nesi-docker-base:$BASE_VERSION
docker push ghcr.io/lbrick/nesi-ondemand-vnc/nesi-ondemand-vnc:$VNC_VERSION
```