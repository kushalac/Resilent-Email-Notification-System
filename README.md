# Resilient Email Notification System Overview

This project implements a resilient email notification system using Kafka, React, Spring, and MongoDB. It includes features such as priority settings, user-based sequencing, single/bulk messaging, read operations, real-time cancellation, and detailed event logging.
![Main Page](https://github.com/kushalac/Resilent-Email-Notification-System/blob/master/images/Main-page.png?raw=true)


## Setup

### Kafka Setup

1. Download Kafka from the [official website](https://kafka.apache.org/downloads) and extract the files.
2. Navigate to the Kafka directory.
3. Start Zookeeper:
```javascript
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
```
5. Start Kafka server:
```javascript
.\bin\windows\kafka-server-start.bat .\config\server.properties
```

### Development Environment
1. Install SpringTool Suite (STS) or any preferred IDE for Spring development.
2. Clone this repository to your local machine.
3. Open the project in your IDE.
4. Configure your MongoDB connection in `application.properties`.
5. Run the application.

## User Stories / Functional Requirements

- **Send notifications:** The system should be able to send notifications to users.
- **Priority settings:** Users should have the option to prioritize notifications and toggle application notifications on or off, categorizing messages from settings.
- **User preferences:** The system should adjust notification sequence based on the user's saved preferences.
- **Single/bulk notification:** Support for sending both single/simple and bulk notification messages.
- **Read operations:** Provide read-only or read and operation features for notification messages.
- **Real-time cancellation:** Users should be able to cancel any notification at any time by removing their user ID from the client-side application.
- **No duplicate notifications:** Ensure that the same notification is not delivered twice.
- **Event logging:** Log every notification dispatched, delivered, opened, seen, unsuccessful, and canceled.

## Technologies Used

- **Kafka:** Message broker for scalable and resilient messaging.
- **React:** Frontend framework for user interfaces.
- **Spring:** Backend framework for application development.
- **MongoDB:** NoSQL database for data storage.

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
