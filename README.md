Slack Clone Login Screen
Technology
This demo uses:

CometChat Pro 3.0.10
Firebase
React
Material Icons
node v16.14.2
slatejs
emoji-picker-react
Todo list
 update message input box to support emoji，markdown and attachments
 enable users to expand/collapse channel list and DM list
[] enable users to create a new chat from the clicking on sidebar button
[] refactor the code to use redux
[] refactor the code to use docker
[] refactor the code to use typescript
Running the demo
To run the demo follow these steps:

Head to CometChat Pro and create an account
From the dashboard, add a new app called "slack-clone"
Select this newly added app from the list.
From the Quick Start copy the APP_ID, APP_REGION and AUTH_KEY. These will be used later.
Also copy the REST_API_KEY from the API & Auth Key tab.
Navigate to the Users tab, and delete all the default users and groups leaving it clean (very important).
Download the repository here or by running git clone https://github.com/TheCrowd/slack-clone.git and open it in a code editor.
Head to Firebase and create a new project
Create a file called app.config.js in the src folder of your project.
Import and inject your secret keys in the app.config.js file containing your CometChat and Firebase in this manner.
// For Firebase JS SDK v7.20.0 and later, measurementId is optional
const firebaseConfig = {
  apiKey: "xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx",
  authDomain: "xxx-xxx-xxx-xxx-xxx-xxx-xxx",
  databaseURL: "xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx",
  projectId: "xxx-xxx-xxx",
  storageBucket: "xxx-xxx-xxx-xxx-xxx",
  messagingSenderId: "xxx-xxx-xxx",
  appId: "xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx",
  measurementId: "xxx-xxx-xxx",
};

const cometChat = {
  APP_ID: "xxx-xxx-xxx",
  AUTH_KEY: "xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx",
  REST_KEY: "xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx",
  APP_REGION: "xx",
};

export { firebaseConfig, cometChat };
Make sure to exclude app.config.js in your gitIgnore file from being exposed online.
Run the following command to install the app.
    npm install
    npm start
