# Docker basic commands 

Before getting into specific Docker functionalities it is important that you become familiar with the Docker main commands. This because in many cases you will have to interact manually with your containers in tasks such as listing the current running apps and built images, executing non-primary commands into those containers, reading logs, taging and pushing images to remote repos, etc. In addition, Docker is mostly managed from CLI and this is really relevant every time you get a new project which makes use of this approach.

To complete this, here are some questions that might help you get an idea of whether skip or not this step:
1. Have you ever pulled an image pubished on the Docker hub?
2. Have you used *docker run* for executing any container?
3. How do you run a container in background?
4. Can you expose and map ports between a Docker container and your host machine?
5. How can you read a docker container's logs and debug whether something is going wrong?
6. Could you run and interact with a multi-command container such as redis? 
7.  Do you know how to build a Docker image including tag names, environtment variables, build args, resource constraints, etc.?

In case you could not answer any of the above questions, here is a challenge for you. Do not forget that Docker needs to be installed on your machine. If you prefer to avoid this for now, login into [play-with-docker.com](https://labs.play-with-docker.com/) for getting a ready-to-run instance. However, you will need to install it locally for the rest of this ramp-up:

1. **Pull a Redis image from Docker Hub and make it run**. Docker has a public repository with a bunch of Docker images with some dependencies already installed which will make you run your apps faster and easier. In this first interaction, you are required to download and run a container with Redis preinstalled. Once done, you will see what Redis shows as output when it is running. As you may know, there are some differences between running a program as usual against doing it as a daemon, how about running your Redis container in background?
2. **Connect to the Redis CLI from your host**. Even though every Docker container has a default command, you could run multiple commands inside your container when possible. Redis brings two main commands, *redis-server* which runs the engine and *redis-cli* through which you can interact with that engine. Your goal is to get into the redis container shell and run *redis-cli* from inside, as well as making sure that you can *save* and *get* some values from it. As a means to do so, you should know that Docker allows you to synchronize your terminal with the container I/O.
3. **Show logs from a running container**. Having a container running **in background** brings a tradeoff, you cannot watch the logs output at once. So, when you need to see what is happening inside the container, Docker lets you extract its logs. Now, your task is to save those logs into a file called *myredis.log*. 
4. **Create a custom image from a running container**. There are sometimes when we have a fully configured and customized container, and we need to create an image based on it. Having that image, you can upload it to any container registry such as [Docker Hub](https://hub.docker.com/) or [ECR](https://aws.amazon.com/es/ecr/). Get into your Redis container shell, make some changes followed by commiting it into an image porperly tagged. Finally push your image to the container registry of your choice.

**Note**: This challenge is optional. Feel free to skip it if you are comfortable with Docker CLI commands.