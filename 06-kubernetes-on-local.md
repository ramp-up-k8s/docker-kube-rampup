# Kubernetes on local
Although we have the app running in Kubernetes, this is just the beginning. We rarely deploy things using just the cli tool at least this is for testing purposes. The real first step towards a real-world use case is making this a piece of code:

1.  **Create a manifest for each microservice.** As you saw in the workshop of the last challenge, all of the Kubernetes objects can be defined in YAML files commonly called manifests. Your first task for this challenge is converting those pods and services into manifests. Additionally, you will create a custom namespace and group those resources in that namespace. 
2.  **Move your pods to Deployment controllers**. Pods are ephemeral which means they are not designed to run forever, and when a Pod is terminated it cannot be brought back. That's why you need to transform those pods into [Deployment controllers](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/). While creating your objects, there are several components to take into account. For instance, you might need an *init container* in charge of checking whether your dependencies are ready to respond to your main app. Here are some features you must consider:
    1.  We can limit how much memory and CPU a single pod can use. Research about how to do it and implement it yourself.
    2.  Change the number of replicas to scale up the number of pods for one particular Deployment.
    3.  Choose a deployment strategy and argument why is this the best choice.
    4.  When your deployment is running, list all the pods and select one. Run the command `kubectl delete pod pod_name -n <your_namespace>`. The pod will be deleted. List again all the pods. You should see that kubernetes creates a new pod. This happens because the Deployment controller makes sure that the number of replica that you specified are the replicas running.
3. **Replace the way you expose the and change it for an ingress.** In the installation of Minikube you were requested to install an ingress controller, this for having a better way to expose your application endpoint to outside the cluster. Use this approach instead of using a service for this. In what scenario is this a better way?
   
**Note:** Remember to push all your work to a repository.
