# Blood4U - Blood Bank Management Application

A full-stack web application designed to streamline blood donation processes, facilitate coordination between donors, hospitals, blood banks, and organizations, and enable real-time blood stock management.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Project Architecture](#project-architecture)
- [Database Structure](#database-structure)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Project Modules](#project-modules)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)

---

## Project Overview
**Blood4U** is a blood bank management system developed using the **MERN stack (MongoDB, Express, React, Node.js)**. It addresses the challenges in coordinating blood donations, allowing multiple user roles (Donor, Hospital, Organization, Admin) to access tailored functionalities for managing and requesting blood stock.

The application is designed to:
- Enable secure donor registrations.
- Facilitate real-time blood stock updates.
- Allow hospitals to request specific blood types and track requests.
- Provide organizations with the tools to organize donation events.

---

## Features
1. **Multiple User Roles**: 
   - **Donor**: Can register, view donation history, and find nearby donation events.
   - **Hospital**: Can view and request specific blood types.
   - **Organization**: Can create and manage blood donation events.
   - **Admin**: Has full control over users, blood stock, requests, and event management.

2. **Real-Time Blood Stock Management**:
   - Blood banks can update and monitor blood stock levels in real-time, providing immediate updates to hospitals on availability.

3. **Secure Registration and Authentication**:
   - User authentication is managed with **JWT (JSON Web Tokens)** for secure access control.

4. **Event Management**:
   - Organizations can create donation events, while donors can view and register for these events.

5. **Hospital Requests**:
   - Hospitals can check blood availability and place blood requests to address urgent needs.

6. **Admin Dashboard**:
   - A comprehensive dashboard for the admin to monitor all activities, including user management, blood stock updates, and request handling.

---

## Technologies Used
- **Front-End**: React.js
- **Back-End**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JSON Web Tokens (JWT)
- **Real-Time Updates**: WebSocket or similar technology

---

## Project Architecture
The Blood4U application follows a **MERN stack architecture** with the following layers:
- **Client-Side (React)**: Handles user interactions, data display, and API calls.
- **Server-Side (Express & Node.js)**: Processes client requests, manages business logic, and communicates with the database.
- **Database (MongoDB)**: Stores data on users, blood stocks, donation events, and hospital requests.

---

## Database Structure
Here’s a breakdown of the key MongoDB collections used:

- **Users**: Stores information for donors, hospitals, organizations, and admins.
- **BloodStock**: Tracks real-time availability of various blood types across locations.
- **BloodRequests**: Manages hospital requests for specific blood types.
- **DonationEvents**: Records details of upcoming and past donation events.
- **DonorHistory**: Keeps a record of each donor’s history and eligibility status.
- **AdminLogs**: Logs activities performed by the admin for monitoring purposes.

---

## Installation & Setup

To run this project locally, follow these steps:

### Prerequisites
Ensure you have the following installed:
- **Node.js** and **npm**
- **MongoDB**

### Steps
1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/Blood4U.git
    cd Blood4U
    ```

2. **Install Server-Side Dependencies**:
    ```bash
    cd server
    npm install
    ```

3. **Install Client-Side Dependencies**:
    ```bash
    cd ../client
    npm install
    ```

4. **Set Up Environment Variables**:
    - Create a `.env` file in the root directory of both `client` and `server`.
    - Add necessary environment variables such as MongoDB URI, JWT secret, and others.

5. **Start the Server and Client**:
    - In the server directory, run:
      ```bash
      npm start
      ```
    - In the client directory, run:
      ```bash
      npm start
      ```

6. **Access the Application**:
    Open your browser and go to `http://localhost:3000` to view the application.

---

## Usage
1. **Donor**: Registers, views donation history, and checks nearby events.
2. **Hospital**: Logs in to view and request blood stock.
3. **Organization**: Creates donation events and tracks participants.
4. **Admin**: Manages all system activities, overseeing users, stocks, and events.

---

## Project Modules
1. **User Management**: 
   - Handles role-based registration and login with secure access control.

2. **Blood Stock Management**:
   - Real-time updates on blood stock levels across locations.

3. **Hospital Blood Requests**:
   - Allows hospitals to place requests for specific blood types and track fulfillment.

4. **Event Management**:
   - Allows organizations to set up blood donation events and enables donors to register.

5. **Admin Dashboard**:
   - Provides a comprehensive view of the system for the admin to monitor and manage activities.

---

## Future Improvements
Potential enhancements for the Blood4U application include:
- **Mobile Application**: A mobile version to make the platform more accessible.
- **Notification System**: Real-time notifications for donors and hospitals on request statuses and eligibility.
- **Data Analytics**: A reporting feature for administrators to analyze donation trends and stock availability.

---

## Contributing
Contributions are welcome! If you’d like to contribute to Blood4U, please fork the repository and create a pull request with your proposed changes.

1. **Fork the repository**
2. **Create a new branch**:
   ```bash
   git checkout -b feature-name
