# nesi-ondemand-base

Builds the following docker images:

- [ghcr.io/nesi/nesi-docker-base](https://github.com/nesi/nesi-ood-base/pkgs/container/nesi-docker-base)
- [ghcr.io/nesi/nesi-ondemand-vnc](https://github.com/orgs/nesi/packages/container/package/nesi-ondemand-vnc)


## Installation on deployment host

```
# Install ansible dependencies ...
ansible-galaxy role install -r requirements.yml -p ansible/roles
```

## Manual run

Setting the below will allow you to do a manual run locally

```
export PKR_VAR_docker_username=aValue
export PKR_VAR_docker_password=someValue
```

Then run the following
```
packer build ./packer/base-template.pkr.hcl
```