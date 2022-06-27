[__Back to home__](../index.md)

# Specifications 

The task is left up to us to decide how we use data available to us and what analysis we want to do. It is necessary to consider that a user might not have multiple apps/datasets that encompass some of the things we might want to draw correlations between, e.g., user might only have data for their sleeping patterns, which would mean we cannot analyse how their sports performance is affected by this. As such we discussed a couple approaches to this. The first was potentially to use machine learning on other historical data of similar profiles so that we could provide a dataset for our missing parameter given we obtain a few details from the user (could be height, weight, gender, age etc.). Another idea was to limit our analysis to just using the given data from which we could provide some interesting insights (looking at someone’s sleeping patterns and recommending how they might improve their quality of sleep). We will also have to consider how the user is able to view data as the idea is to create a custom dashboard for users to select what they want to observe depending on what insights are available given their data. 

 The idea is to create a website to view this on with the potential to move this to an app in the future. For the backend Node.js was agreed on while frontend would be implemented using React. We will also need to have a database which we can pull data from to display our analysis on the website. This will also involve authentication via the backend to ensure use of a Terra account. From this we were able to decide on factors to consider:

**Accurate and relevant data**:


**Straight forward User Interface in adequation with terra's design**:

**Interesting  dashboard for health insights**: