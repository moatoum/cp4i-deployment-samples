# Instructions to Run the Driveway Dent Deletion Demo
This set of instructions is a step-by-step guide to running the Driveway Dent Deletion demo.

You do not need to have expertise in using the Cloud Pak for Integration (CP4I), although previous experience will be useful.

Similarly for using the individual integration capabilities used in this demo: IBM App Connect, IBM MQ or IBM API Connect.

## Demo Scenario
This demo shows how to use multiple capabilities of CP4I working together to provide a complete integration solution which is deployed using a fully automated CI/CD pipeline.

![Driveway Dent Deletion Solution](images/DrivewayDentDeletionSolutionDiagram.png)

A full description of the demo scenario is [here](Scenario.md)

### Key Demo Highlights
* Integration solution using multiple CP4I capabilities.
* Deployed using CI/CD OpenShift pipeline
* Shows 'live' updating of integration versions without downtime
* Shows 'rollback' of deployments without downtime
* Shows HA resilience and scaling of the integration solution, recovering from failed pods, scaling of deployments etc.

## List of Ingredients / Things you will need
If you already have these, skip right on! Otherwise click the links to find out how to get them...
### An Instance of IBM Cloud Pak for Integration (CP4I)
You'll need version 2020.2.1 or later. You can run CP4I on the IBM cloud, on another cloud of your choice (e.g. AWS, Azure, GCP), on the Redhat Marketplace or on your own infrastructure.

If you need to get an instance of CP4I to run this demo, see [here](../../Docs/Environments/README.md)
