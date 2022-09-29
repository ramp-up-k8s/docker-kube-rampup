# Kubernetes on the cloud

You have made a substantial advance in setting up your cluster locally to deliver the application up and running, but we can push the envelope. Now, we will learn how to take all of these resources to the cloud for giving a deployment accessible to everyone. For so, most of the cloud providers have support for this technology and those are pretty similar.

This challenge aims to move your effort to our previously created Kubernetes cluster in AWS (Yeah! We did all the dirty work for you). Request access to the training cluster and a namespace in it, all of this can be managed by your trainer. After you have a connection to the cluster, you will be able to complete the following tasks:

1. **Run the applications as it is.** This is one of the advantages of using Kubernetes, the configuration is what it is anywhere (almost all the time XD) Make the same manifests run in this new cluster and test it works successfully.
2. **Package all your manifests into a Helm chart.** When you are in a productive environment, you don't want to edit your manifests and hardcode the values each time you need to deploy the application, you could even need different values for each environment (dev, prod...). That's why we need to transform all these manifests into one or more [Helm](https://helm.sh/docs/) charts (packages), Helm allows you to create templates and parametrize your applications for making them reusable in different environments with different parameters each time.
3. **Terraform your helm chart (optional).** For going one step further, Terraform has a Helm provider. Why? Well, most apps don't work alone, they usually have external dependencies such as databases, Redis, Kafka, and other services outside the K8S cluster. Using Terraform you can integrate those dependencies and call their outputs from your helm chart to make all the deployment processes work synchronously. Let's integrate your helm chart with Terraform and create a Terraform module to deploy your app.

**Note:** Do not forget to use a VCS always.
