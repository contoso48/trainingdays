# Day 2 Azure Development

## Welcome

This day is about getting your hands dirty with application development in Azure. We will dig into the topics

- Serverless
- Storage
- Messaging

## Challenges

- [Challenge 0:  Setup your system](challenges/00-challenge-setupvm.md) *(45 min.)*
- [Challenge 1: Serverless](challenges/03-challenge-serverless.md) *(45 min.)*
- [Challenge 2 (optional): Messaging](challenges/04-challenge-messaging.md) *(45 min.)*
- 💎 *[Breakout 2: Add a serverless microservice to our sample app and include messaging](challenges/05-challenge-bo-2.md)* 💎 *(45 min.)*
- [Optional Challenge 3: Azure Web Applications](challenges/01-challenge-appservice.md) *(45 min.)*
- 💎 *[Breakout 1: Deploy the Azure Dev College sample application to Azure](challenges/02-challenge-bo-1.md)* 💎 *(30 min.)*


### Application

We are going to use the sample application to get to know all the Azure services throughout the workshop. The application is a **Simple Contacts Management** (SCM). You can - surprisingly - create, read, update and delete contacts with it. Currently, we will be storing the contacts in an in-memory database. On *Day 3* we will learn about the various database services of Azure and add proper persistance to our services.

Later that day, we will add a event driven service that modifies images in a storage account an *Azure Storage Account* (Blob). We will also create thumbnails of the images in background via an *Azure Function* which will automatically be triggered through an *Azure Storage Queue*.

The frontend for the application is a small, responsive Single Page Application written in *Vue.js* (which is one of the popular frameworks at the moment). We will be using the cheapest option to host a static website like that namely *Azure Blob storage*.

To make things more tangible, here are some screenshots of the application:

- Welcome page of the app
  ![day2_1](./images/day2_goal1.png "day2_1")
- List of contacts
  ![day2_2](./images/day2_goal2.png "day2_2")
- Detail view of a contact
  ![day2_3](./images/day2_goal3.png "day2_3")

### Result 

At the end of the serverless lab 
 - Create a event drive function which reacts upon file uploads and resized an image 
 - Create a logic app which consumer an Service bus topic and places the content into a storage account 
