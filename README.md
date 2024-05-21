# Smart India Hackathon Workshop
# Date:21-5-2024
## Register Number:212223230189
## Name: SANJAYKUMAR N B
## Problem Title
E-Waste Facility Locator
## Problem Description
Website that tells you the location of the nearest e-waste collection and recycling facility. Offers educational pop-ups on the harmful components of your e-waste and their effects on the environment and human health if not disposed correctly. There could be an option to input the model of your old device and earn credit points relative to the amount of precious metals recovered from the device if disposed correctly.
## Problem Creater's Organization
Ministry of Environment

## Idea
Location-Based Facility Finder: An interactive map and search feature to locate the nearest e-waste facilities.

## Proposed Solution / Architecture Diagram
Create an interactive web application that allows users to easily locate the nearest e-waste collection and recycling facilities. The core feature of the application will be a map-based interface where users can search for facilities based on their current location or a specified address. The application will also provide detailed information about each facility, including contact information, operational hours, and types of e-waste accepted.

```
User Interface (Frontend)
       |
+------------------+
|                  |
|   React.js       |
|   Google Maps API|
|   Material-UI    |
|                  |
+------------------+
       |
   REST API
       |
+------------------+       +----------------+
|   Node.js        |       |                |
|   Express.js     |-------|   MongoDB      |
|                  |       |                |
+------------------+       +----------------+
       |
+------------------+
|  Firebase Auth   |
|  Geolocation API |
+------------------+
```

## Use Cases
User Location-Based Facility Finder:

Scenario: Users want to find the nearest e-waste collection and recycling facility.
Goal: Input location to receive a list of nearby facilities, complete with contact details and operational hours.
Educational Pop-Ups:

Scenario: Users need information on the harmful components in their e-waste.
Goal: Interactive pop-ups explain the risks associated with harmful materials and the benefits of proper recycling.
Rewards System:

Scenario: Users want to dispose of an old electronic device and earn rewards.
Goal: Input device model to estimate the amount of precious metals that can be recovered, earn points accordingly, and redeem them for rewards.

## Technology Stack
Frontend
React.js: For building a dynamic and responsive user interface .
Google Maps API: To provide interactive mapping and location search capabilities .
Material-UI: For implementing a consistent and aesthetical design system.
Backend
Node.js: For handling server-side operations and API requests.
Express.js: A web application framework for building RESTful APIs.
MongoDB: A NoSQL database to store facility data, user information, and search logs .

## Dependencies
npm packages:

react, react-dom: For UI components.
axios: For handling HTTP requests.
express: For server and API creation.
mongoose: For MongoDB object modeling.
firebase: For authentication services.
APIs:

Google Maps API: Requires an API key for access.
Firebase Authentication: Requires setup and configuration in Firebase Console.
Custom API for precious metals calculation: Needs to be developed and hosted.
