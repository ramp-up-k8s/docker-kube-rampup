# Kubernetes first steps

Now that you have a clear idea of how to deploy an application environment using Docker containers, you were able to perceive that the more complex it becomes the harder it is to deliver your app consistently and easily. The most popular tool to automate deployment, scaling, and management of those containers is [Kubernetes](https://kubernetes.io/). In this challenge, we will use [Minikube](https://minikube.sigs.k8s.io/docs/) to set up our local Kubernetes cluster.

For this challenge, you are required to create a Kubernetes cluster on local in charge of managing the To-Do app.

1. This cluster should have at least 2 worker nodes and 1 ingress controller such as [nginx-ingress-controller](https://docs.nginx.com/nginx-ingress-controller/)
2. Now that we have our first kubernetes cluster, let's put it in action. As we know kubernetes might look like an oddball to you the very first time, we will help you in this first step with a short guide:
   - Complete our Kubernetes first steps workshop: https://github.com/ramp-up-k8s/k8s-first-steps-ws
3. Do a short research on what is every type of service for and document it. e.g. What is a *LoadBalancer* service? When should I use it against a *ClusterIP*?
4. When you already have a clear idea of how to run simple apps in Kubernetes, apply this knowledge to our To-Do application. Create a bash script where you launch a pod and a service (**if needed**) for each To-Do's microservice using the docker images that you previously pushed to the registry (**All using just kubectl**). How are they going to communicate to each other? Pay attention to the environment variables. The purpose of this item is making sure you get completely familiar with the cli tool since you'll interact with this a lot. Show evidence of the entire application running after you run the script.
