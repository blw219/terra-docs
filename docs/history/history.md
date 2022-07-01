[__Back to home__](../index.md)

# User Needs

The Client (Terra) asked us to create a Dashboard Web App, which itegrates with their pre-existing Terra Widget. This Dashboard would allow users to connect their wearable accounts via the Terra Widget, and then view meaningful health data and analysis via graphs, charts, suggestions based on the users health data etc. The Dashboard should also be simplistic and easy to use, hiding the complexity of the widget and connections of different wearable data models.

# Verification Protocols

During the design process, we met regularly with the client, especially during the beginning of the project.
These discussion helped mold the direction of the project and gave us clearer understanding of the goals of the project combined with our unique suggestions, to produce the final product. 
These discussions were recorded in the [meeting minutes](meeting/meeting.md) section of the project

# Design History 

The idea is to create a website to view this on with the potential to move this to an app in the future. For the backend Node.js was agreed on while frontend would be implemented using React. We will also need to have a database which we can pull data from to display our analysis on the website for which we are using MONGODB This will also involve authentication via the backend to ensure use of a Terra account. From this we were able to decide on goals to achieve by each weekly meeting which are as follows: 
 

## 1 - Basic Design (front end :log in back end : stores the log in details)
Our first step was to understand how the terra's API works and the use of webhooks. The first draft was just a basic login page and the back end was set up to store the log in detail requesting a session ID and Opening the widget which will allow us to pull the user data later.

One of the key features of Terra is pushing data asynchronously to an endpoint. It allowed us
receive data whenever it is available by the user's wearable without having to query it
Receive large amounts of data without worrying about the payload size in a classic HTTP request

<img width="850" alt="Screenshot 2022-07-01 at 13 48 32" src="https://user-images.githubusercontent.com/58296040/176892000-8f526ed4-6b4c-4844-9a5b-dbab834f4678.png">

## 2 - authentication flow : getting the widget open and verifying connected wearables
Now that we were able too receive data from Terra, we had to connect the users wearable accounts to the webapp. Using Terra's widget, a user can login and connect their different wearables and complete the authentification process to allow Terra to access their wearable data.

<img width="750" alt="terra-widget" src="https://user-images.githubusercontent.com/58296040/176870192-3aa8bd0e-fce7-452a-ad4b-145d78a7e9fa.png">

![image](https://user-images.githubusercontent.com/58296040/176873703-3999b7ec-36e8-4520-a8e8-24834ead6838.png)

**Authentification Flow diagram**

 


## 3 - Implemented the database flow to store and retrieve data & started adding unique ids for each session (each sessions we generatean id through a hash and store it with wearable id show code) 
Our database: TODO BE TEAM 
<img width="700" alt="database2" src="https://user-images.githubusercontent.com/58296040/176876800-d199ed7c-d7d9-4246-91d2-205d1077d3e6.png">
<img width="700" alt="database1" src="https://user-images.githubusercontent.com/58296040/176876828-12e0c3f9-20ec-406d-b167-8b3fca539318.png">



## 4 - After having a fixed architecture for our Front end and Back end we Redesigned the user interface  with template given by Terra.
![template](https://user-images.githubusercontent.com/58296040/176888020-f142da59-cfed-4e54-90e8-1a994e3e839e.png)

Upon getting the template the company wanted us to follow, we came up with our final design to meet their criterias.
We changed colors, added logos and refactored our dashboard to display data in a similar way, while keeping some of our ideas.


<img width="761" alt="Screenshot 2022-07-01 at 12 11 19" src="https://user-images.githubusercontent.com/58296040/176875051-c2d590e1-94a2-4793-abb9-e3b020a00a2c.png">



## 5 - Health observations and suggestions 

While our main goal was to display data from diifferent sources for the user, we also wanted to offer a deeper analysis. Going further into the data analysis and doing rearch on health and fitness guidlines and trends, we were able to generate suggestions to improve their health. These suggestions can be related to their nutrition , sleep, sport performance but also stress and anxiety and overall wellbeing.
![MicrosoftTeams-image (1)](https://user-images.githubusercontent.com/58296040/176888079-c7a73ed6-d11d-4d11-8145-53866a16ed16.png)

## 6 - analytics pages for further analysis and visualisation 

In line with idea to dig deeper in our analysis, an analytics page has been added which displays more details to the user on their data.
Our dashboard was mainly separated in 3 blocks :<br />

- nutrition (calories consumed) <br />
- health (sleep , heart rate) <br />
- performance (calories burned, daily activities) <br />


The analytics page is a place for the user to have access to more information and deeper analysis and suggestions, over more datasets and aspects of the users health . For example the user can have a breakdown of its macro-nutriments per day but also his exact sleeping pattern ...

<img width="458" alt="Screenshot 2022-07-01 at 12 09 13" src="https://user-images.githubusercontent.com/58296040/176874941-6fbe13ff-81ef-4d00-8c8f-6bebd40fb307.png">

