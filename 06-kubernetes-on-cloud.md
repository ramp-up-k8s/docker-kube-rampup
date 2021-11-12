# Kubernetes on the cloud

You have made a substantial advance setting up your cluster locally to deliver the application up and running, but we can push the envelope. Now, we will learn how to take all of these resources to the cloud for giving a deployment accessible from everyone. For so, most of the cloud providers have support for this technology and those are pretty similar.

This challenge aims to set up the cloud environment on which the project will run using the Kubernetes services your preferred cloud provider supplies:

1. **Create a diagram.** This should reflect the design of the infrastructure you will create in the next steps. 
2. **Bring your cluster to the cloud.** Make sure you have all the necessary infrastructure in place for your cluster to be deployed correctly and securely: VPCs, subnets, security groups, etc. Research which Kubernetes implementation your cloud provider delivers as a service and deploy your Kubernetes cluster. A Kubernetes integration with your provider's other services would be appreciated. This means you can evaluate which Kubernetes components could be complemented or replaced by your cloud provider's services, e.g. secret management, volumes, load balancers, etc. All of this is up to you. 
3. **Code your cloud infraestructure.** Once you are clear about your application infrastructure, including the Kubernetes cluster and the services you are going to use from it and your cloud provider, it is time to give infrastructure as code a try. Investigate which tool best fits your needs and constraints, then replicate your deployment but using IaC. You should now be able to deploy or destroy your environment using just a couple of commands.

**Note:** Do not forget using a VCS always.
