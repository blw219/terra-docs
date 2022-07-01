[__Back to home__](../index.md)

# Access WebSite, or Host Locally

The Terra Health Dashboard App can either be used via the hosted URL (Insert URL here) : 
Or you can run and host the website on your local machine
Both Methods will be explained below

# Access Website

Using the URL: (Insert URL here) , you can access the Terra Dashboard on your computer or mobile deevice.
Just go to the URL, or copy it into your browser.
Then login as a guest.
A newe window will open with the Terra widget
Sign in with any of your wearable accounts, which are listed in the widget
Go back to the main Dashboard page and observe your health analysis on the main or analytics page 


# Host Website Locally

Clone the repository to your local machine using git clone (Insert URL here) .
Go into the project directory.

## Run these commands in terminal

### `npm install`

Go into the front end project folder, and run the command 'npm install' to Download and Update all Project Dependencies for the frontend folder
Once it has completed, go back out into the main project folder, and follow the same steps to Download dependencies in the backend folder, inside the main folder

### `npm start`

Open 2 terminals, and in one go into the frontend folder, and in the other the backend folder.
Then run the command 'npm start' in both terminals, which runs the app in the development mode.
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

## Once Hosted

Once you can see the webpage in your browser, login as a guest
A terra widget will open and allow you to connect your wearable accounts to the dashboard
Once youve connected at least one wearable, you can view your health analysis data in the dashboard main page
