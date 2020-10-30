# Instructions to Run the Weather Chatbot Demo
This set of instructions is a step-by-step guide to running the demo.

You do not need to have expertise in using the Cloud Pak for Integration, although previous experience will be useful.

WIP - more to follow.

## Assets in the repo
* App Connect flows, contained in `/assets/app-connect-flows`
  * `Tickets_StormIncWeatherAPI`: Implements an API that checks the weather on a date and location, and opens a ServiceNow ticket if it determines that a storm has happened
  * `classifyImagedV4.yaml`: Implements an API that recognises an image, determines it value, and appends this information to a ServiceNow ticket
    * [More detail on the implementation of this flow](./doc/classifyImages.md)
  * `IncidentSummary`: retrieves summary information about a claim from the ServiceNow ticket
* API Connect flows, contained in `/assets/api-connect-flows`
  * `chatbot_***.yaml`
    * Each of these flows act as a routing layer between a Watson Assistant Webhook invocation and the App Connect APIs (see above)
    * They are needed to support different environments that the API Connect flow could be running in
    * chatbot
* Watson Assistant skill
  * `/assets/watson-assistant-skills/skill-Stormy-Insurance.json`: implements the Watson Assistant front-end to the demo
