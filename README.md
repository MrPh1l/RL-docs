# Rocket league mapmaking website documentation
A guide by Mr Swaggles

## Deployment
**NOTE**: These steps will currently only work for the main `rocketleaguemapmaking.com` domain, as it hasn't been made 
customisable yet. If you wish to view this locally, see the [contribution](./docs/menu/contribute.md) documentation.

This site can be executed as a docker container on the host machine.
1. [Install Docker-CE](https://docs.docker.com/engine/install/) on the host machine. Docker (non-ce) should also work but is not tested.
2. Clone this repository.
3. Navigate into the root of the repository.
4. Execute `sh deployment/build_and_deploy.sh <BUILD_VERSION>`, e.g. `sh deployment/build_and_deploy.sh 0.1.0`.
  - This container will run in the background, and you can access the website.
  - To view all docker containers, execute `docker ps -a`, which are ordered by age.
  - To view the NGINX logs of a container, execute `docker logs <container_name>`.
  - To stop the service, execute `docker stop rlmm`
6. Access the site at the correct URL (`rocketleaguemapmaking.com`).

## Contributing documentation
Read the [contribution](./docs/menu/contribute.md) documentation for guidelines when contributing.
