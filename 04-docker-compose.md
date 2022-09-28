# Docker Compose

Now that you have managed to deploy a multi-tier application using only Docker, you should realize it is pretty cumbersome to connect each container with its dependencies including volumes, networks, ports, environment variables, etc. Part of this ramp-up is to make you acquire skills when it comes to synchronizing services. Now then, during the development cycle we are always looking for practices which make us work effectively. Therefore, tools have been developed that allow us to synchronize these services in a faster way. 

For this challenge you will have to replicate what you deployed in the last challenge (building from Dockerfile) but using [Docker Compose](https://docs.docker.com/compose):

1. **Sync your containers using Docker Compose.** Now that you have at least five containers, in addition to their network. You must create a Docker Compose YAML file in which all of those resources will be defined. Once created, you should be able to pull the needed base images, build your custom ones, set environment variables, run and connect all the containers and other stuff only using one command.
2. **Manage several environments.** Learn what features you should set in your docker-compose file to have it ready for a fast development environment. How about production? Is that possible? Any pros and cons?
