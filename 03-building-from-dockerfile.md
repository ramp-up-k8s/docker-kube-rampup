# Building images from Dockerfile

Once you get familiar with the Docker basic commands, it is time to start building new images ready to run our apps. The way you provision a new image is throughout Dockerfile. Here is where you download a base snapshot, add arguments and environment variables, copy and configure files and set your main command. 

For this challenge, your will have two goals:

1. Download the *Movie Analyst* repos and add Dockerfiles able to build a fully configured image for running the apps. You have to take into account that these containers need some ports binded to your host machine in order to connect to each other.
2. Now that you have your images ready, make them run synchronously ensuring that the API is responding to all the UI requests.  

**Note**: This connection could be easily done by using a multi-container app definer, but this is an approach that we will treat leater.