[__Back to home__](../index.md)

# Specifications 

The task is left up to us to decide how we use data available to us and what analysis we want to do. It is necessary to consider that a user might not have multiple apps/datasets that encompass some of the things we might want to draw correlations between, e.g., user might only have data for their sleeping patterns, which would mean we cannot analyse how their sports performance is affected by this. As such we discussed a couple approaches to this. The first was potentially to use machine learning on other historical data of similar profiles so that we could provide a dataset for our missing parameter given we obtain a few details from the user (could be height, weight, gender, age etc.). Another idea was to limit our analysis to just using the given data from which we could provide some interesting insights (looking at someone’s sleeping patterns and recommending how they might improve their quality of sleep). We will also have to consider how the user is able to view data as the idea is to create a custom dashboard for users to select what they want to observe depending on what insights are available given their data. 

 The idea is to create a website to view this on with the potential to move this to an app in the future. For the backend Node.js was agreed on while frontend would be implemented using React. We will also need to have a database which we can pull data from to display our analysis on the website. This will also involve authentication via the backend to ensure use of a Terra account. From this we were able to decide on factors to consider:

# Robust algorithm
Our statiistical algorithm runs each tme new data is uploaded , searchng for underlyijng relaionshps in activity, sleep, weight and other habits. Using Linear regresssion , scatter plots , impact scorres or sampliing peiods.

# TODO ADD BACKEND

# Frontend

# Easy to and understand and use Webapp

- The WebApp was designed with ease of use and simplicity in mind. One of the main puproses of the App is to hide the complexity behind the Terra API and the user's different data models, and allow the user to connect and understand our health data analysis with no prior programming knowledge.
- As such, all the user has to do is sign in with their own wearable account details, and everything is displayed in on the dashboard main page and analytics page, with clear analysis and breakdowns

# Health Data Analysis and Suggestions over multiple data sets
 
- We want to use the users health data from the wearables they have connected to make meaningful analysis and suggestions
- Depending on how many wearables the user connects, we intend to display more meaningful and intricate analysis the more data sets we are provided.
- We then want to compare and discover patterns and correlations between the datasets to explain possible health problems and suggest improvements to aspects of their health
- If the user provides only 1 wearable account, then we only have 1 dimension to analyze, and can therefore draw on public health guidelines to analyze and make suggestions to the user
- We will then ask the user, if they have available, to connect more wearable accounts, so that we can display and analyze in more dimensions, correlations between their health data


# Connect different wearables

- Using the widget session provided by Terra, a user can login to their wearable accounts on a new browser/pop up window
- On loggin in with their wearable accounts, the app pings Terra's database for the users health data from the wearables autherized
- We can then display the data in meaninfgul ways through grapsh, suggestions, breakdowns ect on the main Dashboard Page and Analytics Page

## Dashboard And Analytics Cards

The final website is split into a couple pages that display user data in multiple ways with different plots and analysis. It shows nutrition, activity and sleep data. The home page has three plots with one for each of these sectors, which focuses on one key aspect of each. The first is a line chart that shows the user's calorie intake over the course of thirty days as well as displaying the averge intake for the thirty days. The second focused on the calories burned over the last thirty days, similarly using a line chart and showing an average. Hours slept per night was the final plot, which also used a line chart and presented an average. Above all three plots are suggestions that depend on the data shown. For example, if the average calorie intake was considerably lower than the average calories burned the suggestion is along the lines of being awake for more hours can increase one's appetite. These suggestions also include praise if the user is deemed to have healthy data, such as a high amount of calories burned would result in a suggestion congratulating the user on having an active lifestyle.

On the analytics page there are seven plots with three of them for sleep data, two for nutrition and two for activity. The sleep plots consisted of a bar chart and two line charts. The bar chart displays a full analysis on a user's sleep with datasets for total sleep, light sleep, deep sleep and REM sleep over a month. This is shown as four sets of four bars, which are averages for each variable for each week over a month with monthly averages for each displayed above. This plot is built with the ability to remove datasets from the plot by clicking on the monthly average if a user wants to focus on a couple or one particular aspect of their sleep. The next plot shows maximum, average and minimum heart rate while sleeping for each night over a week. This plot also has the ability to remove maximum and minimum heart rates by clicking on labels above the plot. The final line chart shows the user's sleep efficiency over a month. Sleep efficiency is percentage given by looking at the amount of time spent sleeping over the total time in bed by using total sleep times and awake times for each night (The recommendation here is to have 80% or higher).

In the nutrition section there is a pie chart with two rings representing the user's intake of protein, carbohydrates and fat compared with the daily guidelines given by the government. On this plot categories can be removed by clicking on the legend and numbers are shown by hovering over each segment. Next to this is a table with columns showing food groups, user intake, daily guidelines, percentage difference and a suggestion for each. The food groups shown here are protein, carbohydrates, fat, sodium, sugar and calories. Suggestions are given by looking at the percentage difference with a certain margin allowed for a healthy disparity. These range from positive encouragement to suggestions to either reduce or increase your intake for each group. All values are taken from average of daily recordings over a week.

The last section is activity, which has a horizontal stacked bar chart and a vertical bar chart. The stacked chart tracks vigorous activity minutes over a month and displays the daily averages for each week, giving a percentage breakdown of activity for each week. The other chart has two datasets of steps and distance walked and run for each day over week with a total given for each above. This also has the option to remove each dataset by clicking on the monthly total.

The website also comes with a sidebar that can be opened and has links for the home page, the analytics page, the terra widget where users sign into their wearable accounts as well as a login page to sign into their account with our website.

