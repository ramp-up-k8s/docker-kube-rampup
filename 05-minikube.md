# Kubernetes on local

Now that you have a clear idea of how to deploy an application environment using Docker containers, you were able to perceive that the more complex it becomes the harder it is to deliver your app consistently and easily. The most popular tool to automate deployment, scaling, and management of those containers is [Kubernetes](https://kubernetes.io/). In this ramp-up, we will use [Minikube](https://minikube.sigs.k8s.io/docs/) to set up our local Kubernetes cluster.

For this challenge, you are required to create a Kubernetes cluster on local in charge of managing the Movie Analyst.

1. **Create a pod for each app.** While creating your pods, there are several components to take into account. For instance, you might need an *init container* in charge of checking whether your dependencies are ready to respond to your main app. You will also have to define what kind of objects you want to create according to your needs, how much resources your containers are going to spend, among other things.
2. **Sync all your pods.** Create services, daemon-sets, namespaces and everything you need to synchronize and support your cluster. 
3. **Manage your DB with the best practices.** As mentioned in previous sections, in many cases you will have to make your data persistent which is not fully supported using only containers. Find the best way to deal with databases using Kubernetes.  

