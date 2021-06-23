---
layout: container
name: rsync
github: https://github.com/autamus/registry/blob/main/containers/r/rsync/spack.yaml
versions:
- 3.2.2
updated_at: 2021-06-22T20:14:37.927180423Z
size: 33MB
description: An open source utility that provides fast incremental file transfer.
container_url: https://github.com/orgs/autamus/packages/container/package/rsync

---
# rsync
```bash 
Download        : docker pull ghcr.io/autamus/rsync
Compressed Size : 33MB
```

## Description
An open source utility that provides fast incremental file transfer.

## Usage
### Pull (Download)
To download the latest version of rsync run,

```bash
docker pull ghcr.io/autamus/rsync:latest
```

or to download a specific version of rsync run,

```bash
docker pull ghcr.io/autamus/rsync:3.2.2
```
### Run
To run the container as an application run,
```bash
docker run --rm ghcr.io/autamus/rsync rsync --version
```

or to run the container in an interactive session run,
```bash
docker run -it --rm ghcr.io/autamus/rsync bash
```

### Mounting volumes between the container and your machine
To access files from your machine within the rsync container you'll have to mount them using the `-v external/path:internal/path` option.

For example,
```bash
docker run -v ~/Documents/Data:/Data ghcr.io/autamus/rsync rsync /Data/myData.csv
```
which will mount the `~/Documents/Data` directory on your computer to the `/Data` directory within the container.

## HPC
If you're looking to use this container in an HPC environment we recommend using [Singularity-HPC](https://singularity-hpc.readthedocs.io) to use the container just as any other module on the cluster. Check out the SHPC rsync container [here](https://singularityhub.github.io/singularity-hpc/r/ghcr.io-autamus-rsync/).