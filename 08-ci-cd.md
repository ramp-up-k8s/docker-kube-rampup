# CI/CD
In real-world projects, there are lots of features to work on. From maintenance tasks to creating new ones. All of these changes are meant to be developed with good quality and in the fastest way possible. As part of this ramp-up, we encourage you to learn a good way to ensure every change follows the necessary phases to deliver a product bug-free, fast and reliable. All of this is as automated as you can.


## CI
In the first part you will design and set up your CI pipeline:

1. **Setup a CI Service** Using your knowledge, deploy a CI service such as Jenkins, Travis, Github Actions, AWS CodePipeline, Azure DevOps to implement your CI/CD process there.
2. **Design and pipeline for your continuous integration process.** Even though Docker eases your artifact-building process, you will need to define through which phases your product will pass before being sure it is ready for deployment. Make a diagram taking into account the kind of artifact you deliver and where to place it to allow your Kubernetes cluster to pull it.

## CD
At the end of the CI process, you will end up with an artifact (certainly a docker image) fully tested and ready to be deployed. Now your task consists of deploying that artifact in our Kubernetes cluster:

***Note:** be careful with AWS credentials, avoid publishing them in any public source such as github, try to use some strategy such as secrets.*

1. **Research and learn about deployment strategies** used commonly for Kubernetes projects and choose one to implement your project.
2. **Design and implement your pipeline.** Think of the kind of objects you will need to touch in your cluster to have your application up and running. As well as the implementation of the **deployment strategy** that you chose for your deployment.
