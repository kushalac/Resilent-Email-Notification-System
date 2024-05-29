# Resilient Email Notification System Overview

This project implements a resilient email notification system using Kafka, React, Spring, and MongoDB. It includes features such as priority settings, user-based sequencing, single/bulk messaging, read operations, real-time cancellation, and detailed event logging.

![Main Page](https://github.com/kushalac/Resilent-Email-Notification-System/blob/master/images/Main-page.png?raw=true)

## Architecture

![Architecture](https://github.com/kushalac/Resilent-Email-Notification-System/blob/master/images/Architeture.png?raw=true)

## Setup for Resilient Email Notification System Backend

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
5. In `EmailSender.java` update your `email` and `App password`.
6. Run the application.

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

## Setup for Resilient Email Notification System Frontend

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm install react-scripts --save-dev`

We gain access to essential tools provided by Create React App (CRA). These tools include a development server for hot reloading (npm start or yarn start), build scripts for production optimization (npm run build or yarn build), and testing capabilities (npm test or yarn test). react-scripts streamlines development, improves code quality through testing, and prepares your application for deployment, making it a crucial component for efficient React development.

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
