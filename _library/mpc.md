---
layout: container
name: mpc
github: https://github.com/autamus/registry/blob/main/containers/m/mpc/spack.yaml
versions:
- 1.1.0
updated_at: 2021-05-26T06:49:43.936080258Z
size: 30MB
description: Gnu Mpc is a C library for the arithmetic of complex numbers with arbitrarily
  high precision and correct rounding of the result.
container_url: https://github.com/orgs/autamus/packages/container/package/mpc

---
# mpc
```bash 
Download        : docker pull ghcr.io/autamus/mpc
Compressed Size : 30MB
```

## Description
Gnu Mpc is a C library for the arithmetic of complex numbers with arbitrarily high precision and correct rounding of the result.

## Usage
### Pull (Download)
To download the latest version of mpc run,

```bash
docker pull ghcr.io/autamus/mpc:latest
```

or to download a specific version of mpc run,

```bash
docker pull ghcr.io/autamus/mpc:1.1.0
```
### Run
To run the container as an application run,
```bash
docker run --rm ghcr.io/autamus/mpc mpc --version
```

or to run the container in an interactive session run,
```bash
docker run -it --rm ghcr.io/autamus/mpc bash
```

### Mounting volumes between the container and your machine
To access files from your machine within the mpc container you'll have to mount them using the `-v external/path:internal/path` option.

For example,
```bash
docker run -v ~/Documents/Data:/Data ghcr.io/autamus/mpc mpc /Data/myData.csv
```
which will mount the `~/Documents/Data` directory on your computer to the `/Data` directory within the container.

## HPC
If you're looking to use this container in an HPC environment we recommend using [Singularity-HPC](https://singularity-hpc.readthedocs.io) to use the container just as any other module on the cluster. Check out the SHPC mpc container [here](https://singularityhub.github.io/singularity-hpc/r/ghcr.io-autamus-mpc/).