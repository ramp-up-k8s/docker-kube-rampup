# Welcome

An *agile delivery culture* such as DevOps requires to be continuously evolving. It implies that many tecnologies will emerge for the sake of increasing the efficiency throughout the process of development and operations. Because of that, this ramp-up is meant to encourage you to improve your skills with containerization and orchestration.

First, Docker has become popular since it reduces significantly the amount of repetitive configuration tasks, giving us the advantage of having an easy-to-run and portable application development. Once you are completely familiar with the Docker ecosystem, you will encounter a multi-container application which will need a great effort in orchestration. Here is where Kubernetes brings its power automating the deployment, scaling and management of those containers.

Following the same methodology used for other ramp-ups on this platform, this brings a set of challenges meant to show beginners the basics of the two technologies mentioned above which are leading in the DevOps area nowadays.

## Projects

In order to complete the challenges and let you focus on what matters to us about this ramp-up, you will be provided with a project to work with. 

### 1. To-Do app
- This application is a To-Do webapp based on a microservices architecture model where each service is developed in a different language: VueJS, Go, NodeJS, Springboot and Python.
- For this application, you will not have to write any code in order to make it work as expected. But, you will find it is kind of tricky to orchestrate all of these services while trying to run all of them at once.

~~~ bash
# using SSH
git clone git@github.com:ramp-up-k8s/todo-app.git
~~~
or 
~~~ bash
# using HTTPS
git clone https://github.com/ramp-up-k8s/todo-app.git
~~~
