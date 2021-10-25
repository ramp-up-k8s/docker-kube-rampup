# Kubernetes on local

Now that you have a clear idea of how to deploy an application environment using Docker containers, you were able to perceive that the more complex it becomes the harder it is to deliver your app consistently and easily. The most popular tool to automate deployment, scaling, and management of those containers is [Kubernetes](https://kubernetes.io/). In this step, we will use [Minikube](https://minikube.sigs.k8s.io/docs/) to set up our local Kubernetes cluster.

For this challenge, you are required to create a Kubernetes cluster on local in charge of managing the Movie Analyst.

1. **Create a pod for each app.** While creating your pods, there are several components to take into account. For instance, you might need an *init container* in charge of checking whether your dependencies are ready to respond to your main app. You will also have to define what kind of objects you want to create according to your needs, how much resources your containers are going to spend, among other things.
2. **Use Kubernetes for building the best environment.** Make use of Kubernetes services and other components to bring your application to a high availability environment. What about some containers for log monitoring? Use namespaces for setting up visibility among your app layers. You are free to add what you consider in order to give some support to your cluster. 
3. **Connect to your DB from Kubernetes.** As mentioned in previous sections, in many cases you will have to make your data persistent which is not fully supported using only containers. Should you use Kubernetes *volumes* and containerized engines? Network filesystems? Or definitely treat them externally? Find the best approach to deal with databases using Kubernetes.
