# Project Description:

> Tasks performed
* Created Health Bot Instance
* Create a LUIS resource in azure
* Chose a authoring resource by signing in to the LUIS portal
* Created a LUIS coversation app - Appointment Booking
* Added entities to the conversation app - doctor_type 
* Created intents for the conversation app - BookAppointment
* Trained, Tested angd Published the conversation app
* Integrated LUIS into Azure Health Bot by
   * Imported the Booking appointments template scenario
   * Copied the required keys from the LUIS portal
   * Created a new language model in the health bot
   * Fetched intents from LUIS and map them to a scenario
   * Tested the language model in Web Chat

* Creating a scenario for an interrupting bot- Intermediate Bot 1
* Creating a model for an interrupting bot
* Creating a breaking scenario - Intermediate Bot 2
* Creating a model for a breaking scenario.

The required screenshots are attached in the images folder.

The demo could be seen at [Demo](https://eastus.healthbot.microsoft.com/account/nd-health-bot-hn3uvcx)


Various terminologies used here:
>Health Bot

The Azure Health Bot service is a cloud platform that empowers developers in healthcare organizations to build and deploy compliant virtual health assistants and health bots. These tools take advantage of AI and help healthcare organizations to improve processes and reduce costs.

The service combines built-in medical intelligence with natural language capabilities and more. It allows healthcare organizations to give people access to trusted and relevant healthcare services and information.

> LUIS models

LUIS models are great for natural language understanding. They understand broader intentions and improve recognition. They also require an HTTPS call to an external service. LUIS models return a confidence score based on mathematical models used to extract the intent.

LUIS is deeply integrated into Health Bot and supports multiple LUIS features, such as:

* Bing Speller: Provide your Bing Speller subscription key in the endpoint URL to pass all utterances through a spell check before undergoing processing by the LUIS application. For more information, see [Bing Speller](https://docs.microsoft.com/en-us/azure/cognitive-services/bing-spell-check/overview).
* Staging: Use the staging version of your LUIS application if you want to prevent testing from affecting the learning of your production LUIS application. For more information on publishing your LUIS application, see [Production and Staging slots](https://docs.microsoft.com/en-us/azure/cognitive-services/bing-spell-check/overview).
* Verbose responses: Typically, the response from your LUIS application includes only the highest scoring intent for the model. To include all intents and their respective scores in the response, use the Verbose setting.

When you create a LUIS model, you'll need an account with the [LUIS.ai service](https://www.luis.ai/home) service.

>Interrupting scenario

An interrupting scenario causes a break in the flow of the scenario. It allows us to jump between two scenarios.

Initially, the main scenario is where the bot runs. Due to a keyword that it encounters, the bot switches to the sub-scenario that's defined as a model. After the sub-scenario is complete, the bot switches back to the main scenario with an interrupt message that's defined during the configuration.

>Breaking Scenario

A breaking scenario also causes a break in the flow of the scenario.

Initially, the main scenario is where the bot runs. Due to a keyword that it encounters, the bot switches to the sub-scenario that's defined as a model. After the sub-scenario is complete, the bot does not switch back to the main scenario.





