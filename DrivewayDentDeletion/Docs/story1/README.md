# Driveway Dent Deletion Demo
## Story 1: Deploy the Solution using a CI/CD pipeline

When integration components have been built and unit tested, we want to create container images for them and then deploy them all together using a deployment pipeline that deploys and configures all of the components automatically without manual intervention.

![Basic Pipleline Overview](images/DDDBasicPipelineDeploy.png)
*(ToDo: Update this screenshot)*

Our solution consists of 4 App Connect integration flows, each as its own independent deployment/replica set, together with an MQ queue manager with a number of queues.

Here we are going to build 5 container images, one for each component and then deploy them all to the ICP4i runtime.

The flow is this:
Create all of the integration artefacts and place them into github.

Create a Pipeline and deploy that pipeline to CP4i

Create a WebHook which will detect when a change has been made to the github repository and start the pipeline to create a new build.

The pipeline will create container images for each of the integration artefacts then deploy the images to CP4i, ensuring that they are all correctly bound together.
