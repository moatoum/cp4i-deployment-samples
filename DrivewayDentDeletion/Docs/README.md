# Instructions to Run the Driveway Dent Deletion Demo
This set of instructions is a step-by-step guide to running the Driveway Dent Deletion demo.

You do not need to have expertise in using the Cloud Pak for Integration (CP4I), although previous experience will be useful.

Similarly for using the individual integration capabilities used in this demo: IBM App Connect, IBM MQ or IBM API Connect.

## A note on the instructions...
We appreciate that we have different audiences, ranging from 'I just want to get the demo running as fast as possible' to 'I want to use this as a learning exercise and explore all the details'

We've tried to keep the 'end-to-end flow' as simple as possible and provide lots of 'Deeper Dive / More Info / Why did we do this?' links off to the side.

## Demo Scenario
This demo shows how to use multiple capabilities of CP4I working together to provide a complete integration solution which is deployed using a fully automated CI/CD pipeline.

![Driveway Dent Deletion Solution](images/DrivewayDentDeletionSolutionDiagram.png)

A full description of the demo scenario is [here](Scenario.md)

## Key Demo Highlights
* Integration solution using multiple CP4I capabilities working together
* Fully containerised/Kubernetes deployment
* Deployed using CI/CD OpenShift pipeline
* Shows 'live' updating of integration versions without downtime
* Shows 'rollback' of deployments without downtime
* Shows HA resilience and scaling of the integration solution, recovering from failed pods, scaling of deployments etc.
* Shows end-to-end tracing capabilities

## List of Ingredients / Things you will need
If you already have these, skip right on! Otherwise expand the links to find out how to get them...
<details>
<summary>An Instance of IBM Cloud Pak for Integration (CP4I)</summary>

You'll need version 2020.2.1 or later.
<br><br>
You can run CP4I on the IBM cloud, on another cloud of your choice (e.g. AWS, Azure, GCP), on the Redhat Marketplace or on your own infrastructure.
<br><br>
If you need to get an instance of CP4I to run this demo, see [here](../../Docs/Environments/README.md)
</details>
<details>
<summary>A github account and repository</summary>

As we're going to be using piplelines for this demo, we'll be storing the artefacts that we want to deploy in github.<br><br>

The way that the demo works is that when you commit a change to github, this automatically starts the pipeline to build and deploy the change.<br><br>

As you need to make changes, you'll need to make a copy of our repository (know as 'forking') and then make changes to your copy/fork.

We'll give you instructions as to how to do this but you will need a github account. These are free to create (you can use a free email address if you wish and full instructions are at www.github.com)

If you already have a github account, you can use that.
</details>
