[__Back to home__](../index.md)

# Meeting Minutes

Overview of KEY decisions taken:

- Tech stack


# 27th April 2022 - Internal Meeting

## **Agenda**:

**What they do**: Terra links data originating from wearables from multiple different companies (including Garmin, Fitbit, Peloton etc.) and makes them accessible to developers on a single API. This sees them act as a middleman between wearables and developers by creating an easy link between the two that can be used to analysis on multiple health and wellness parameters. 

 

**What they want us to do**: The task they have for us is to present graphics that depict interesting data analysis based on historical data. This is left rather open-ended for us to choose what analysis we want to do but will need to be presented on a dashboard with plots and potentially insights/correlations on the given data. The goal of this is to entice less tech savvy customers to observe the potential of what Terra can do with their platform and present this visually to elicit a more immediate and positive response from someone who might not understand the concept fully to start with. Regardless of the level of understanding of their platform it is a logical next step in the evolution of their company. 

 

**Factors to consider**: The task is left up to us to decide how we use data available to us and what analysis we want to do. It is necessary to consider that a user might not have multiple apps/datasets that encompass some of the things we might want to draw correlations between, e.g., user might only have data for their sleeping patterns, which would mean we cannot analyse how their sports performance is affected by this. As such we discussed a couple approaches to this. The first was potentially to use machine learning on other historical data of similar profiles so that we could provide a dataset for our missing parameter given we obtain a few details from the user (could be height, weight, gender, age etc.). Another idea was to limit our analysis to just using the given data from which we could provide some interesting insights (looking at someone’s sleeping patterns and recommending how they might improve their quality of sleep). We will also have to consider how the user is able to view data as the idea is to create a custom dashboard for users to select what they want to observe depending on what insights are available given their data. 

 

**What we actually have to do**: The idea is to create a website to view this on with the potential to move this to an app in the future. For the backend Node.js was agreed on while frontend would be implemented using React. We will also need to have a database which we can pull data from to display our analysis on the website. This will also involve authentication via the backend to ensure use of a Terra account. From this we were able to decide on goals for the first week which are as follows: 


## **Minutes**:

* Obtain an understanding of Terra’s API and use of webhooks 
* Brainstorm dashboard ideas and how we want to display them 
* Setup GitHub repository 
* Start to develop the basics of the frontend and backend for the website 
* Setup authentication 
* Start work on AWS database 


# 5th May 2022 - Meeting with Terra

## Completed: 
* Front-end - basic setup 
* Backend - framework setup
* Basic login - basic UI
* Request session ID - successfully requested session ID
* Opening widget

 

## To-Do: 

**Trello**: Plan all tasks and setup who does what 

**Frontend**: 
* Website design 
* Data Visualised 
* Decide tools 

**Backend**: 
* Authorisation 
* Store user data 

**Additional stuff (Optional)**: 

* Heroku: Is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud. 
* Material UI: Offers a comprehensive suite of UI tools to help you ship new features faster. 
* Ngrok: Is a globally distributed reverse proxy fronting your web services running in any cloud or private network, or your machine.  

 

**Things to do (for the following week)**: 

* Connecting to widget – Zion / Kai 
* Authorise wearable account – Zion / Kai 
* Pull data - Ruwan 
* Display - All 
* Local database for data - Boon 
* Compare frameworks - Myriam 

