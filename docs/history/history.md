[__Back to home__](../index.md)

# Design History 

The idea is to create a website to view this on with the potential to move this to an app in the future. For the backend Node.js was agreed on while frontend would be implemented using React. We will also need to have a database which we can pull data from to display our analysis on the website for which we are using MONGODB This will also involve authentication via the backend to ensure use of a Terra account. From this we were able to decide on goals tto achieve by each weekly meeting which are as follows: 
 

Week 2: 
    • Obtain an understanding of Terra’s API and use of webhooks 
    • Brainstorm dashboard ideas and how we want to display them 
    • Setup GitHub repository 
    • Start to develop the basics of the frontend and backend for the website 
    • Setup authentication 
    • Start work on AWS database 

Week 3
	• Set up the Front-end
	• Set up the Backend
	• Configure a basic login
	• Request session ID
	• Opening widget
	• Pull some user data

week 4
	• Display some basic analysis
	• Database
	• Plan for front end layout
 
Trello: Plan all tasks and setup who does what
 
Frontend:
    • Website design
    • Data Visualised
    • Decide tools
 
Backend:
    • Authorisation
    • Store user data


week 5
Note down mistakes in debugging for other users in this doc/OneNote
 
Frontend:
 
    • Fix display issues
    • Visualize user data on graphs
    • Notify which wearables to connect to see data
    • Nutrition, Performance, health graphs: calories, calories burned, sleep
 
Backend:
 
    • Pull relevant data
    • Link user ID to wearable IDs in database and backend
 
Database:
 
Storing relevant user data in structured format


week 6
Habitdash: take a look at competition, maybe take inspiration

Things to do:

Frontend:

	• More graphs: other metrics plotted
	• Remove unnecessary icons ok
	• Add time scale ok ?
	• Correct reference links ok
	• Format plots ok
	• Colours (customise) ok
	• Login Page ?
	• Use tailwind element (loading symbol..)

Backend:

	• Finish automatic retrieval on connection
	• Optimise the storing data

Uni stuff:

	• Leaflet
	• Poster

By 6th June surpass Habitdash 

Health:
Sleep pattern  https://ouraring.com/blog/sleep-score/

Weight ? Compared to
Heart rate with performance 

week 6
Use Tailwind for premade spinners when loading data


week 7
Deliverables:

	• Add detailed sections for each category: Different data representation e.g. food groups, pie chart, nutrition, performance, health
	• Suggestions for heart health, diversify workouts, tracking workout habits (heart rate is going down weekly with the same workout), heart rate during sleep correlating with workouts, workouts late at night maybe affecting sleep, comparing intake of calories against calories burned daily
	• Data Analysis: observations, meal sleep, sleep vs alcohol, trends between different data
	• Fix Issues
Matching designs



1-Basic Design (front end :log in back end : stores the log in details)
SC zion
2- authentication flow : getting the widget open and verifying connected wearables
terra's diagram https://docs.tryterra.co/docs/quick-setup 
https://docs.tryterra.co/reference/rest-authentication

![widget terra](../../images/database1.png?raw=true)


3-basic visual data representation 
sc from gc
4- Implemented the database flow to store and retrieve data & started adding unique ids for each session (each sessions we generate an id through a hash and store it with wearable id show code) link the ressource zionteams
database 1: storring the data to be repeated to display
2:connecting our unique iids to the all of the users wearable ids
5- Redesign with template habitdash
show new design and template given by alex
without suggestions

7- Health observations and suggestions 
sc suggestions 
8-analytics pages for further analysis and vsualisation 
sc