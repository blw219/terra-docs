[__Back to home__](../index.md)

# Code and Resources


## Unique User Session ID
![image](https://user-images.githubusercontent.com/59968760/176776662-846d01df-5243-4c5e-8c77-7c4dcc99e32d.png)

- Each time a user starts a session by going to the website in their brower, a unique session ID is created and passed within the states of the React DOM
- This ID is created using a sha256 Hash, using the Current time and a random pertubated string as a key, meaning 2 users would have to access the website at the exact same second ( very unlikely ) and be given the exact same random string, to have the same ID. This is quite impossible
- The use of a Hashing ID is to anonamize their userID and the connected wearables on the database, IN CASE of a breach or leak, instead of having a simple 0-x ID created based on the number of registered users, and to provide users with privacy guarantees

## User Suggestions

![image](https://user-images.githubusercontent.com/59968760/176885032-8be90755-447d-49a9-9dc9-424e47b051b6.png)
![image](https://user-images.githubusercontent.com/59968760/176894689-893a8129-444c-4c4a-b94c-1ca8477af9fc.png)

- Our Suggestions engine automatically finds correlations and relations between different data sets from different wearables.
- The available data sets are stores in DashboardMoz class state, and passed to the General Suggestions file
- Here, we use a large match case statement, to outout different suggestions based on the type of suggestion we want to provide
- Then based on the available datasets, we can detect averge/outlier trends in the user's health data, based on scientific knoweldge of the human body, to generate meaningful suggestions back to the main Dahsboard Class, where they are outputted on the page

## Connect wearable accounts to unique user session

![image](https://user-images.githubusercontent.com/59968760/176895581-05b472b5-159b-42b5-a04a-cb9419842f99.png)

- On Guest login, or upon clicking the terra widget icon on the sidebar, users will be taken to a new browser page with the Terra Wdiget
- Here they can login and connect any of their wearable accounts to their current session

![image](https://user-images.githubusercontent.com/59968760/176895812-aafd013b-15ac-46ed-91a3-10d045885b8d.png)

- On successful closing of the window, a delete signal is sent to the backend, to delete the users unique session id

## Terra Integration
- [https://docs.tryterra.co/integrating-with-terra](https://docs.tryterra.co/integrating-with-terra)

## React App (frontend):
- [https://github.com/facebook/create-react-app](https://github.com/facebook/create-react-app)

## Authentication Setup
- [https://www.digitalocean.com/community/tutorials/how-to-add-login-authentication-to-react-applications](https://www.digitalocean.com/community/tutorials/how-to-add-login-authentication-to-react-applications
)

## NodeJS Tutorial
- [https://www.youtube.com/watch?v=zb3Qk8SG5Ms&list=PL4cUxeGkcC9jsz4LDYc6kv3ymONOKxwBU](https://www.youtube.com/watch?v=zb3Qk8SG5Ms&list=PL4cUxeGkcC9jsz4LDYc6kv3ymONOKxwBU)

## MongoDB
- [https://www.mongodb.com/docs/](https://www.mongodb.com/docs/)

## Tailwind Dashboard
- [https://github.com/cruip/tailwind-dashboard-template](https://github.com/cruip/tailwind-dashboard-template)
- [https://www.smashingmagazine.com/2020/02/tailwindcss-react-project/](https://www.smashingmagazine.com/2020/02/tailwindcss-react-project/)
- [https://www.ceos3c.com/web-development/react-and-tailwind-beginner-guide/](https://www.ceos3c.com/web-development/react-and-tailwind-beginner-guide/)
- [https://frontbackgeek.com/how-to-add-tailwind-css-in-react-js-application/](https://frontbackgeek.com/how-to-add-tailwind-css-in-react-js-application/)
- [https://tailwindcss.com/docs/customizing-colors](https://tailwindcss.com/docs/customizing-colors)
- [https://tailwind-elements.com/docs/standard/components/charts/](https://tailwind-elements.com/docs/standard/components/charts/)

## Habitdash Dashboard (Competitor)
- [https://habitdash.com/](https://habitdash.com/)

## Leaflet & Poster Design:
- [https://www.canva.com/](https://www.canva.com/)

## Heart Rate Health Analysis:
- [https://www.bhf.org.uk/informationsupport/how-a-healthy-heart-works/your-heart-rate](https://www.bhf.org.uk/informationsupport/how-a-healthy-heart-works/your-heart-rate)
- [https://www.heart.org/en/health-topics/high-blood-pressure/the-facts-about-high-blood-pressure/all-about-heart-rate-pulse](https://www.heart.org/en/health-topics/high-blood-pressure/the-facts-about-high-blood-pressure/all-about-heart-rate-pulse)
- [https://armstrongbodysystems.com/heart-rate-chart/](https://armstrongbodysystems.com/heart-rate-chart/)


## Reaact Component LifeCycle:
-[https://www.educba.com/react-component-lifecycle/](https://www.educba.com/react-component-lifecycle/)
-[https://www.tutorialspoint.com/reactjs/reactjs_component_life_cycle.htm](https://www.tutorialspoint.com/reactjs/reactjs_component_life_cycle.htm)

## React Hooks:
-[https://reactjs.org/warnings/invalid-hook-call-warning.html](https://reactjs.org/warnings/invalid-hook-call-warning.html)
-[https://reactjs.org/docs/hooks-intro.html](https://reactjs.org/docs/hooks-intro.html)
-[https://reactjs.org/docs/hooks-reference.html](https://reactjs.org/docs/hooks-reference.html)

## Reacr UseState Hooks:
-[https://www.w3schools.com/react/react_usestate.asp](https://www.w3schools.com/react/react_usestate.asp)
-[https://reactjs.org/docs/hooks-state.html](https://reactjs.org/docs/hooks-state.html)
-[https://blog.logrocket.com/a-guide-to-usestate-in-react-ecb9952e406c/](https://blog.logrocket.com/a-guide-to-usestate-in-react-ecb9952e406c/)

## React Router:
-[https://www.w3schools.com/react/react_router.asp](https://www.w3schools.com/react/react_router.asp)
-[https://reactrouterdotcom.fly.dev/docs/en/v6/routers/browser-router](https://reactrouterdotcom.fly.dev/docs/en/v6/routers/browser-router)
-[https://medium.com/how-to-react/how-to-use-react-router-in-your-react-js-project-7e1d469a9716#:~:text=How%20to%20use%20React%20Router%20in%20your%20React,useLocation.%20...%205%20useHistory.%20...%206%20Redirect.%20](https://medium.com/how-to-react/how-to-use-react-router-in-your-react-js-project-7e1d469a9716#:~:text=How%20to%20use%20React%20Router%20in%20your%20React,useLocation.%20...%205%20useHistory.%20...%206%20Redirect.%20)
