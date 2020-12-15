# Cognitive Car Insurance Claims Demo - Setting up the Endpoints
Before we can build our API integration, we need to set up the endpoints that we need will integrate to.

This demo doesn’t use emulators, shims or stubs – we’re going to connect to real endpoints in the real-world cloud! You can use these endpoints after this demo to explore more with CP4I and to do other demos – they’re your endpoints to ‘take home and keep’!

All of these endpoints have been deliberately chosen for this demo as they have free versions that we can use – don’t worry, you won’t need a credit card to create them.

We will set up endpoints to connect to:
*	IBM Watson Image Recognition
*	Salesforce
*	IBM Watson Tone Analysis

(If you already have Watson Services and a Salesforce Developer Account e.g. from doing a previous demo, you can skip this section)

Later, we will connect to the following endpoints.

We will set up the language translation in the ‘main’ lab as it is similar to the other Watson services and done in the same place, but we will leave ServiceNow until later.
*	IBM Watson Language Translation
*	ServiceNow


![Shortcut](images/shortcut.png)
<details>
<summary>
"I know how to set up CP4I connectors / I already have connectors"</summary>
If you already know how to set up CP4I connectors, or have some that have already been set up, then great! You can re-use what you have or set them up yourself.

Checklist:
* You will need Salesforce, Watson Visual Recognition, Watson Tone Analyser and Watson Language Translation for the 'main' scenario.
* You will need ServiceNow for the Extension
* All connector accounts in the demo are named 'App Connect Trial' - you don't have to use this convention, but if you want to name your accounts something different, you will need to update the flow definitions.

Once you've set up your connectors, go to the next step which is [Creating The Integration Flow.](creatingTheIntegrationFlow.md)
</details>

## Setting up IBM Watson Services
We will set up Watson Image Recognition, Tone Analysis and Language Translation.

We can set up all three IBM Watson services at the same time.

You will need an IBM Cloud account to do this. You can use your existing one if you wish or you can set up a new one.

IBM cloud access is free and can be provisioned instantly.

Once you have an account, all of the Watson services have ‘lite’ plans which allow you to use them for free – the only restriction is the number of calls you can make per month. Don’t worry, we won’t be getting anywhere near that number – and you won’t get charged if you hit the limit, it will just stop working until the next month.

* Set up Watson Visual Recognition Instructions [here](../../Docs/Connectors/WatsonVisualRecognition/README.md)
* Set up Watson Language Translation Instructions [here](../../Docs/Connectors/WatsonLanguageTranslation/README.md)
* Set up Watson Tone Analyzer  [here](../../Docs/Connectors/WatsonToneAnalyzer/README.md)

## Setting up Salesforce

Instructions for setting up a free Salesforce Developer account and setting up the CP4I SalesForce connector are [here](../../Docs/Connectors/SalesForce/README.md)

## Extension Scenario: Setting up ServiceNow

Instructions for setting up a free ServiceNow Developer account and setting up the CP4I ServiceNow connector are [here](../../Docs/Connectors/ServiceNow/README.md)
## Next Steps:
Once you've set up your connectors, go to the next step which is [Creating The Integration Flow.](creatingTheIntegrationFlow.md)
