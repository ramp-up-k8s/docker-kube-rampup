# Building images from Dockerfile

Once you get familiar with the Docker basic commands, it is time to start building new images ready to run our apps. The way you provision a new image is throughout Dockerfile. Here is where you download a base snapshot, add arguments and environment variables, copy and configure files, set your main command, etc. 

For this challenge, your will have two goals:

1. Download the *To-Do app* repo and add Dockerfiles able to build a fully configured image for running the apps. You have to take into account that these containers need some ports binded to your host machine in order to connect to each other.
2. Now that you have your images ready, make them run synchronously ensuring that the APIs are responding to all the UI requests and they are being deployed after their dependencies are up & running.
3. Keep in mind there are a couple of third-party dependencies which are not in the code such as Redis and Zipkin. 
4. Finally, upload all of the images to any container Registry such as *Docker Hub* or *ECR* properly tagged. 
5. From this point you will have to make use of a source code management tool such as Git or SVN and upload your advance to a hosting platform e.g. Github or RiouxSVN to keep it safe and versioned.

**Note**: This connection could be easily done by using a multi-container app definer like *Docker Compose*, but this is an approach that we will treat later, so let's assume the only tool we have installed is Docker itself.
