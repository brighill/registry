---
layout: container
name: libpng
github: https://github.com/autamus/registry/blob/main/containers/l/libpng/spack.yaml
versions:
- 1.6.37
updated_at: 2021-05-26T06:26:12.118974784Z
size: 27MB
description: libpng is the official PNG reference library.
container_url: https://github.com/orgs/autamus/packages/container/package/libpng

---
# libpng
```bash 
Download        : docker pull ghcr.io/autamus/libpng
Compressed Size : 27MB
```

## Description
libpng is the official PNG reference library.

## Usage
### Pull (Download)
To download the latest version of libpng run,

```bash
docker pull ghcr.io/autamus/libpng:latest
```

or to download a specific version of libpng run,

```bash
docker pull ghcr.io/autamus/libpng:1.6.37
```
### Run
To run the container as an application run,
```bash
docker run --rm ghcr.io/autamus/libpng libpng --version
```

or to run the container in an interactive session run,
```bash
docker run -it --rm ghcr.io/autamus/libpng bash
```

### Mounting volumes between the container and your machine
To access files from your machine within the libpng container you'll have to mount them using the `-v external/path:internal/path` option.

For example,
```bash
docker run -v ~/Documents/Data:/Data ghcr.io/autamus/libpng libpng /Data/myData.csv
```
which will mount the `~/Documents/Data` directory on your computer to the `/Data` directory within the container.

## HPC
If you're looking to use this container in an HPC environment we recommend using [Singularity-HPC](https://singularity-hpc.readthedocs.io) to use the container just as any other module on the cluster. Check out the SHPC libpng container [here](https://singularityhub.github.io/singularity-hpc/r/ghcr.io-autamus-libpng/).