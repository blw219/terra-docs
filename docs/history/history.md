[__Back to home__](../index.md)

# Design History 

The idea is to create a website to view this on with the potential to move this to an app in the future. For the backend Node.js was agreed on while frontend would be implemented using React. We will also need to have a database which we can pull data from to display our analysis on the website for which we are using MONGODB This will also involve authentication via the backend to ensure use of a Terra account. From this we were able to decide on goals to achieve by each weekly meeting which are as follows: 
 

* 1-Basic Design (front end :log in back end : stores the log in details)
Our first step was to understand how the terra's API works and the use of webhooks. The first draft was just a basic login page and the back end was set up to store the log in detail requesting a session ID and Opening the widget whkch will allow us to pull the user data later.

<img width="850" alt="Screenshot 2022-07-01 at 13 48 32" src="https://user-images.githubusercontent.com/58296040/176892000-8f526ed4-6b4c-4844-9a5b-dbab834f4678.png">

* 2- authentication flow : getting the widget open and verifying connected wearables

<img width="750" alt="terra-widget" src="https://user-images.githubusercontent.com/58296040/176870192-3aa8bd0e-fce7-452a-ad4b-145d78a7e9fa.png">

![image](https://user-images.githubusercontent.com/58296040/176873703-3999b7ec-36e8-4520-a8e8-24834ead6838.png)

* 3-basic visual data representation 


* 4- Implemented the database flow to store and retrieve data & started adding unique ids for each session (each sessions we generatean id through a hash and store it with wearable id show code) 
Our database: TODO BE TEAM 
<img width="700" alt="database2" src="https://user-images.githubusercontent.com/58296040/176876800-d199ed7c-d7d9-4246-91d2-205d1077d3e6.png">
<img width="700" alt="database1" src="https://user-images.githubusercontent.com/58296040/176876828-12e0c3f9-20ec-406d-b167-8b3fca539318.png">



* 5- After having a fixed architecture for our Front end and Back end we Redesigned the user interface  with template given by Terra.
![template](https://user-images.githubusercontent.com/58296040/176888020-f142da59-cfed-4e54-90e8-1a994e3e839e.png)

Getting the template the company wanted us to follow we came up with our final design to meet their criterias.
We changed colors , added logos and refactored our dashboard o display data similarly while keeping some of our ideas.


<img width="761" alt="Screenshot 2022-07-01 at 12 11 19" src="https://user-images.githubusercontent.com/58296040/176875051-c2d590e1-94a2-4793-abb9-e3b020a00a2c.png">



* 7- Health observations and suggestions 

While our main goal was to display data from diifferent sources for the user , we also wanted to offer a deeper analysis . Going further into the data analysis and by doing rearch on health and fitness we were able to generate suggestions to improve their  health. These suggestions can be related to their nutrition ,sleep, sport performance but also stress and anxiety .
![MicrosoftTeams-image (1)](https://user-images.githubusercontent.com/58296040/176888079-c7a73ed6-d11d-4d11-8145-53866a16ed16.png)

* 8-analytics pages for further analysis and vsualisation 
In line with idea to dig deeper in our analysis , an analytics page has been added which gives more details o the user on its data.
Our dashboard was mainly separated in 3 blocks :

**nutrition (calories consumed)**
**health (sleep , heart rate)**
**performance (calories burned, daily activities)**

The analytics page is a place for the user to have more information . For example the user can have a breakdown of its macro-nutriments per day but also his exact sleeping pattern ...

<img width="458" alt="Screenshot 2022-07-01 at 12 09 13" src="https://user-images.githubusercontent.com/58296040/176874941-6fbe13ff-81ef-4d00-8c8f-6bebd40fb307.png">

