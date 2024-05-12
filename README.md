# COVID-19 Contact Tracing Flutter Application with Firebase

## Introduction

Amidst the global pandemic, the importance of contact tracing and management has been highlighted to contain the spread of COVID-19. This innovative application, developed with Flutter, is specifically designed for tracing virus-related contacts. During this presentation, we will delve into the application's features, focusing on its architecture, specific views, and security measures to ensure a reliable and secure user experience.

## Application Architecture

This COVID-19 contact tracing application architecture is designed to ensure optimal efficiency while securing data. Here's a detailed overview of its functioning:

### Firebase Collections:

- **Users**: This collection is dedicated to storing information about the application's users. Each user is represented as an individual document within this collection, with fields such as email, password, and username. These data are crucial for enabling secure authentication and personalizing each user's experience.

- **Encounters**: The "Encounters" collection is the core of the contact tracing mechanism. Each encounter between two users is recorded as a document in this collection. Fields include details such as the time, location, and unique identifiers of the two users involved in the encounter. This collection is essential for tracking potential interactions and taking appropriate measures if needed.

### Cloud Firestore Usage:

This application employs Cloud Firestore, Firebase's NoSQL database, to store data flexibly and scalably necessary for the application's proper functioning. Cloud Firestore offers a real-time database structure that allows instant data updates as new encounters are recorded, ensuring real-time responsiveness of the application and enhancing the user experience.

## Application Views

### Overview of Different Views:

- **Home View**
- **Login View**
- **Registration View**
- **Internal View**

#### Home View

The home page offers a clean interface with two distinct buttons: "Login" for existing users and "Sign Up" for newcomers. This simplicity ensures direct navigation, highlighting essential actions right from the start.

#### Login View

The login process is straightforward and secure. Upon clicking the "Login" button from the home page, users are directed to a dedicated view where they enter their credentials, typically email and password. These data are then verified using Firebase's authentication service to ensure a secure connection. If successful, users access the internal view of the application, unlocking all features associated with their account.

#### Registration View

The registration process is designed to be simple and user-friendly. When users select the "Sign Up" button from the home page, they are redirected to a dedicated view where they can provide their personal information, such as email, password, and username. This data is then submitted for validation to ensure its uniqueness and compliance with required criteria.

#### Internal View

The Internal View of the application stands out for its simplicity, focusing on a smooth user experience. It primarily consists of a single key element:

- **Start Tracing Button**: A single button is present, triggering the tracing process upon activation.

## Data Storage in Firebase

Data storage in Firebase, the central pivot of this contact tracing application, relies on two key collections: "users" and "met_with". Each user is represented by a separate document in the "users" collection where sensitive data such as email and password are securely recorded. Similarly, details of encounters between users essential for contact tracing are stored in the "met_with" collection with information such as time, location, and participant identifiers.

## Conclusion

In conclusion, this COVID-19 contact tracing application developed with Flutter and powered by Firebase stands out for its thought-out architecture, simplified features, and enhanced security measures. The main view offers direct access to essential actions for login and registration. The internal view centered on a single start tracing button ensures a seamless experience. Data storage in Firebase's "users" and "encounters" collections managed by Cloud Firestore ensures efficient and secure management. Combining effective data management with rigorous security practices, our application ensures safe and efficient storage of crucial information for COVID-19 contact tracking.
