# Docker - basic commands 

Before getting into specific Docker functionalities you must become familiar with the most common Docker commands. This is because in many cases you will have to interact with Docker using a terminal in tasks such as listing the currently running apps and built images, executing non-primary commands into those containers, reading logs, tagging and pushing images to remote repos, etc. In addition, Docker is mostly managed from CLI and this is relevant every time you get a new project which makes use of this approach.

To complete this, here are some questions that might help you get an idea of whether skip this step or take a look at basic Docker usage:
[ ] Have you ever pulled an image from the Docker hub?
[ ] Have you used `docker run` for executing any container?
[ ] How do you run a container in the background?
[ ] Can you expose and map ports between a Docker container and your host machine?
[ ] How can you read a docker container's logs and debug whether something is going wrong?
[ ] Could you run and interact with a multi-command container such as Redis? 
[ ] Do you know how to build a Docker image including tag names, environment variables, build args, resource constraints, etc.?
[ ] Do you know the purpose of the IT flag in `docker exec`?

In case you could not answer any of the above questions, here is a challenge for you. Do not forget that Docker needs to be installed on your machine.

> :warning: **You are not authorized to install Docker Desktop on your work computer**: Because of Docker's new pricing model we must use an alternative to Docker Desktop, such as installing Docker in WSL for Windows, or Rancher for MacOS.

1. **Pull a Redis image from Docker Hub and make it run**. Docker has a public repository with a bunch of Docker images with some dependencies already installed which will make you run your apps faster and easier. In this first interaction, you are required to download and run a container with Redis preinstalled. Once done, you will see what Redis shows as output when it is running. As you may know, there are some differences between running a program as usual against doing it as a daemon, how about running your Redis container in the background?
2. **Connect to the Redis CLI from your host**. Even though every Docker container has a default command, you could run multiple commands inside your container when possible. Redis brings two main commands, *redis-server* which runs the engine, and *redis-cli* through which you can interact with that engine. Your goal is to get into the Redis container shell and run *redis-cli* from inside, as well as make sure that you can *save* and *get* some values from it. As a means to do so, you should know that Docker allows you to synchronize your terminal with the container I/O.
3. **Show logs from a running container**. Having a container running **in the background** brings a tradeoff, you cannot watch the logs output at once. So, when you need to see what is happening inside the container, Docker lets you extract its logs. Now, your task is to save those logs into a file called *myredis.log*. 
4. **Create a custom image from a running container**. There are sometimes when we have a fully configured and customized container, and we need to create an image based on it. Having that image, you can upload it to any container registry such as [Docker Hub](https://hub.docker.com/), [ECR](https://aws.amazon.com/es/ecr/), etc. Get into your Redis container shell, make some changes (such as adding a new file or installing a new package) followed by committing it into an image properly tagged. Finally, push your image to the container registry of your choice.

**Note**: This challenge is optional. Feel free to skip it if you are comfortable with Docker CLI commands. If you prefer to avoid this, for now, login into [play-with-docker.com](https://labs.play-with-docker.com/) for getting a ready-to-run instance. However, you will need to install it locally for the rest of this ramp-up.
