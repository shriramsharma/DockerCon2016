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
*


## Open Questions?
1. Docker manager node is it transfarable?. Manager could be a single point of failure.
2. Can we take a node out of rotation so that the mesh would stop sending request. Basically healthcheck at runtime
