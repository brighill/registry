---
layout: container
name:  "tensorflow/tensorflow"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/singularity-hpc/blob/main/registry/tensorflow/tensorflow/container.yaml"
updated_at: "2021-05-23 12:56:38.930418"
container_url: "https://hub.docker.com/r/tensorflow/tensorflow"
aliases:
 - "python"

versions:
 - "2.2.2"
 - "2.5.0-custom-op-gpu-ubuntu16"
 - "2.5.0rc0-gpu-jupyter"
description: "An end-to-end open source platform for machine learning."
---

This module is a singularity container wrapper for tensorflow/tensorflow.
An end-to-end open source platform for machine learning.
After [installing shpc](#install) you will want to install this container module:

```bash
$ shpc install tensorflow/tensorflow
```

Or a specific version:

```bash
$ shpc install tensorflow/tensorflow:2.2.2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load tensorflow/tensorflow/2.2.2
$ module help tensorflow/tensorflow/2.2.2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you'll be able to load it to make the following commands accessible:

#### tensorflow-tensorflow-run:

```bash
$ singularity run <container>
```

#### tensorflow-tensorflow-shell:

```bash
$ singularity shell -s /bin/bash <container>
```

#### tensorflow-tensorflow-exec:

```bash
$ singularity exec -s /bin/bash <container> "$@"
```

#### tensorflow-tensorflow-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### tensorflow-tensorflow-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### python
       
```bash
$ singularity exec --nv <container> /usr/local/bin/python
```



In the above, the `<container>` directive will reference an actual container provided
by the module, for the version you have chosen to load. Note that although a container
might provide custom commands, every container exposes unique exec, shell, run, and
inspect aliases. For each of the above, you can export:

 - SINGULARITY_OPTS: to define custom options for singularity (e.g., --debug)
 - SINGULARITY_COMMAND_OPTS: to define custom options for the command (e.g., -b)

<br>
  
### Install

You can install shpc locally (for yourself or your user base) as follows:

```bash
$ git clone https://github.com/singularityhub/singularity-hpc
$ cd singularity-hpc
$ pip install -e .
```

Have any questions, or want to request a new module or version? [ask for help!](https://github.com/singularityhub/singularity-hpc/issues)