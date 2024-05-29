# Resilient Email Notification System Backend Overview

This project implements a resilient email notification system using Kafka, React, Spring, and MongoDB. It includes features such as priority settings, user-based sequencing, single/bulk messaging, read operations, real-time cancellation, and detailed event logging.

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
