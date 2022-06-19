[__Back to home__](../index.md)

# Meeting Minutes

Overview of KEY decisions taken:

- Tech stack

<br />

# 27th April 2022 - First Internal Meeting

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

<br />

# 28th April 2022 - First Meeting with Terra

**Preliminary plan**:
* Front end using react.js run on AWS server 
* Back end using node.js also on AWS server 
* AWS database to store and access all the data 
* Authenticate via Terra API and display basic analysis on webapp 


**Data to display**: 

Ideally have wearables track multiple aspects of health/wellness (e.g. sleep and sports performance), but have to take into account that some users may only track one thing and as a result need to have graphics for just that. 

### **Possible datasets for analysis**: 

**Sleep**: How will we quantify quality of sleep? 
* Factors/variables we could use for this: 
* Hours of sleep, REM and NREM 
* Time awake
* Time taken to fall asleep 
* Amount of awakenings in night 
* Heart rate 
* HRV 
* Timings of sleep, later vs earlier 


Can we use a formula to produce a sleep quality index (1-10)? 

**Sports Performance**: Should focus on cardio (running, cycling etc.) as hard to track weightlifting from wearables' data. 
Factors/variables we could use: 
* Pace (min/km) 
* Heart rate 
* Calories burned 
* Time 
* Distance 
* Route? 

Could use extra variables like VO2 max if wearables provide data 

This would be most straightforward analysis such as just displaying average pace over a couple months. 

**Nutrition**: Very common thing to track, but could be a bit complicated for a project like this due to the numerous variables to track and specialised knowledge needed to inform/analyse on this topic 
Factors/variables to use: 
* Calories (breakdown from all foods and meals) 
* Protein 
* Carbs 
* Fat 
 
Simplest analysis here would be to check different food group intake amounts against recommended amounts for adults. 

**How do we want to analyse multiple datasets**: 
* Sleep Quality vs Sports Performance 
* Sleep times vs Sports Performance? 
* Nutrition vs Sports Performance (this would be complicated) 
* Sports Performance vs Time of day? 
* Sports Performance vs Time of sleep? 

 

How do we want to analyse single datasets (lowkey feels like a Spotify wrapped type-beat): 

**Sports Performance**: 
* Trends for pace 
* Longest distance 
* Fastest pace 
* Most active month/week 

 

**Sleep**: 
* Trends for length of sleep 
* Trends for bedtimes/wake-up times 
* Patterns for sleep quality 
* Following guidance for 7-9 hours recommended sleep? 

**Nutrition**: 
* Comparison with daily recommended amounts of food groups 
* If we have time can customise for each user given parameters of height, weight and dietary goals (bulk/cut) however might be too complicated 


<br />

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

<br />

# 10th May 2022 - Meeting with Terra

## Discussion with Terra:

**Framework design**: 
* Use template or work from scratch? 
* Better to use what is quicker so start with template 

 

**Database**: 
* Authentication: using user_id for each wearable 
* Type of model to be used in database: Most likely same template to be used as Terra data models. 
* Working on structure: looking for how is best to store and pull data and need to find an efficient way to store data rather than storing everything we receive. 
* Services to look at entire file and query which data you actually want to use. 
 

**UI**: 
* Improve visual of the display of the website 

 
**Backend**: 
* Need to sort out how we want to pull data to make it compatible with the data needed for front end plots. 
* Need to sort out different ways we want to request data from Terra 
* Want to find ways to fill in gaps in user profiles from multiple wearables from same users 


**User Profile**: 
* If user has one wearable and therefore insufficient data, might need to input info on frontend to fill info needed to display trends. 


**Plan for next week**: 
* Finish design/come up with scheme for the database 
* Produce a couple useful graphs/plots using data from database 
* ^Above tasks will need to work in parallel to updating the backend 
* Design frontend with framework templates 
* Backend receiving/extracting specific data needed for plots 
* Will need to display these plots on webapps 
* How we choose data to plot (from the data we are given) 
* Find and store generic/average trends/data in the database (need to be able to extract this as well when we choose which data to plot) 
* Come up with high level design for webpage and displaying it (how it actually looks) 

<br />

# 18th May 2022 - Meeting with Terra

**Frontend**: 
* Fix display issues 
* Visualize user data on graphs 
* Notify which wearables to connect to see data 
* Nutrition, Performance, health graphs: calories, calories burned, sleep 

 
**Backend**: 
* Pull relevant data 
* Link user ID to wearable IDs in database and backend 


**Database**: 
* Storing relevant user data in structured format 

<br />

# 23th May 2022 - Internal Meeting

### To do:

* Login page with terra's logo 
* Adjust the 3 graphs done 

**Command bar**:
* Dashboard done 
* Authentification/ Terrra widget done 
* Login done 
* Settings done 

**Others**:
* Welcome bar design done 
* Terra logo instead of the ones on the page
* Color scheme : terra's colors done 


<br />

# 27th May 2022 - Meeting with Terra
 
## Things to do: 

**Habitdash**: 
* take a look at competition, maybe take inspiration  

**Frontend**: 
* More graphs: other metrics plotted 
* Remove unnecessary icons ok 
* Add time scale ok ? 
* Correct reference links ok 
* Format plots ok 
* Colours (customise) ok 
* Login Page ? 
* Use tailwind element (loading symbol..) 

**Backend**: 
* Finish automatic retrieval on connection 
* Optimise the storing data 

**Uni stuff**: 
* Leaflet 
* Poster 

**Notes specific to team**:
* **Health**: 
Sleep pattern  https://ouraring.com/blog/sleep-score/ 
* **Weight**: Compared to heart rate with performance  

<br />

# 31th May 2022 - Meeting with Terra

**To do**:
* Use Tailwind for premade spinners when loading data 

**Deliverables**: 

* Add detailed sections for each category: Different data representation e.g. food groups, pie chart, nutrition, performance, health 
* Suggestions for heart health, diversify workouts, tracking workout habits (heart rate is going down weekly with the same workout), heart rate during sleep correlating with workouts, workouts late at night maybe affecting sleep, comparing intake of calories against calories burned daily 
* Data Analysis: observations, meal sleep, sleep vs alcohol, trends between different data 
* Fix Issues 
* Matching designs 

<br />

# 7th June 2022 - Meeting with Terra

**Backend**: 
* Storing data 
* Automatic flow tweaked 
* Add some data analysis to backend 


**Frontend**:  
* Fix up plots on home page: clear indication of what data is being plotted, fix moving average, add legends, positioning of boxes,  more readable, text ratios 
* Adjust layout of home page: make sure comments are formatted correctly and placed in legible layout 
* Analytics page with real data 
* Observations/suggestions better wording 
* More in depth analysis 
* Use all links/remove unnecessary ones 
* Change graph dates (general button) 

 