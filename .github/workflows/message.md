Please build the container and deploy it to the Sylabs Cloud. It has been two weeks since the last reminder.

Steps to build:

```bash
sudo singularity build container.sif Singularity
```

Steps to deploy:

```bash
singularity remote login
singularity sign container.sif
singularity push container.sif library://apascha1/deploy-singularity-testing/{container name}:{tag}
```
