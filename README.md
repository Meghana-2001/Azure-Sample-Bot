# Azure-Sample-Bot
A basic chatbot based on Azure Technology
page_type	languages	products	description
sample
javascript
nodejs
azure
azure-cognitive-services
These samples create a Study Bot chat client using QnA Maker.
Study Bot (Node.js)

This sample has a StudyBotNode app which was created in Visual Studio, and it has a StudyBotNode_CLI which is the same app but decoupled from Visual Studio and run from the command line. Each app features an embedded bot that you will create in the Azure portal. Create the bot first, then download one of the Study Bot sample apps to embed your bot into. Follow the readme files for the bot and the apps.

These samples create a Study Bot chat client using QnA Maker (with Chitchat) and LUIS. Each query into the chat bot (v4) will be accompanied by relevant search results in an encyclopedia, Microsoft Academic, and a news/blogs section as a study aid. Teachers are able to create their own question and answer FAQs to create a study guide as input for the chat bot if they want it to follow a preferred curriculum. However, demo FAQs are available for this sample, included in the qna-luis-botv4-node/FAQs folder. The focus of this app is to enable a more relevant experience of studying, where students can study a subject with a customized chat bot along with multiple web resources.

FEATURES
QnA Maker with LUIS: There are 3 knowledge bases (created from FAQs in qnamaker.ai) that LUIS directs the user to after a query is received in the chat bot. LUIS has utterances created (in luis.ai) that will allow the right knowledge base to be used. For instance, if the user types in "virus", LUIS knows to go to the biology knowledge base to retrieve a definition (answer) to the user's input. The QnA Maker feature Chitchat has been added to the bot v4 as a 4th knowledge base.

Speech service: Through the microphone button in the webchat, this sample can do Speech-to-Text and Text-to-Speech. When a user clicks the microphone button and speaks in their mic, the speech will be printed to the webchat and the bot will respond with an answer that is audible and printed in the webchat.

The web resources (tabs below the webchat) will take a student query, like "virus", automatically from the webchat queries and return relevant information about it in an encyclopedia, Microsoft Academic, as well as a general Bing search that returns mostly news and blogs on the query.

PREREQUISITIES
Start with the qna-luis-botv4-node sample. Once that is up and running, then download and run the Study Bot app (either the StudyBotNode or StudyBotNode_CLI) sample. The Study Bot depends on the bot you build in the qna-luis-botv4-node sample. Follow the README files in each sample.

Visual Studio 2017+ or a command line (CLI)

The qna-luis-botv4-node is a Node.js web app bot created in the Azure portal.

The StudyBotNode app is a Node/Express Visual Studio app, whereas the StudyBotNode_CLI app uses Express but can be run from the command line.

RESOURCES
QnA Maker Dcoumentation
QnA Maker API V4.0
Add Chitchat to a QnA Maker knowledge base - we don't use this method of enabling a knowledge base (KB) with Chitchat in this sample, because we have more than one knowledge base, so we create a stand-alone KB with Chitchat only. If you only have one KB, then it's preferred to enable it in that knowledge base. For more information on the stand-alone Chitchat KB, refer to the Qna-Luis-Botv4 sample's README.
Language Understanding (LUIS) Documentation
LUIS Programmatic APIs v2.0
LUIS Endpoint API
Azure bot service
Integrating QnA Maker and LUIS bot v4 tutorial, using Dispatch
Speech Services Documentation
