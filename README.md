# DockerCon 2016!!!

## What's new in Docker
* Swarm Mode
* Services
> docker service create
* Scaling
> docker service scale <service-name>=10
* Global Services
* Constraints

### Services
Services -> Tasks -> Containers
> Tasks are basically VMs or Unikernels.

New file format, DAB. This is experimental.

### Routing Mesh
### Security out of the box
* Automatic cert rotation

### Container Healthcheck
>HEALTHCHECK in dockerfile.

### Docker plugin permission model.

## Contributing to docker.
* IRC: docker-dev

## Docker for developers
* > docker compose up

## Docker and containerd
* lightweight Container supervisor

## runC OCI
libcontainer interfaces with cgroups and namespace.
OCI is a standard on how to design and implement containers.
runc is a client wrapper around libcontainer. You need to provide a config.json and root filesystem.
runc will use these two info to run your container. JSON is based on OCI spec.
runc/libcontainer is the library contains all the low level OS stuff.
`ocitools generate` creates a basic config.json to start with.

## Unikernels


## Open Questions?
1. Docker manager node is it transfarable?. Manager could be a single point of failure.
2. Can we take a node out of rotation so that the mesh would stop sending request. Basically healthcheck at runtime
3. DTR, if the base image has any secruity issue like the one that was shown in the keynote. If there are 100 apps base of the base image. Would we need to rebuild and redeloy all the images.
