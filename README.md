# Video-Conferencing

This document provides an overview of a React application that includes routing, authentication, and integration with a backend API.

## Overview

This React application is designed to provide users with various functionalities, including a homepage, dashboard, video conferencing rooms, and a messenger feature. It utilizes React Router for client-side routing, Redux for state management, and integrates with a backend API for authentication and data retrieval.

## Installation

To install and run the application locally, follow these steps:

1. Clone the repository:

     ```git clone https://github.com/MeGaTroNOO7/Video-Conferencing```

2. Navigate to the project directory:

     ```cd Video-Conferencing```

3. Install Dependencies:

     ```npm install```


## Usage

To use the application, follow these steps:

1. Start the development server:

     ```npm start```

2. Open the application in your web browser:

   ```http://localhost:3000```


## Components

The application consists of the following main components:

- **Home**: The homepage component.
- **Dashboard**: The dashboard component.
- **Video**: Component for video conferencing rooms.
- **ChatApp**: Component for messenger feature.

## Routing

The application uses React Router for client-side routing. The main routes are as follows:

- `/home`: Homepage
- `/dashboard`: Dashboard
- `/room/:roomId`: Video conferencing rooms
- `/conversations`: Messenger feature
- `/conversations/:roomId`: Individual conversation

## Authentication

Authentication is implemented using JSON Web Tokens (JWT). Users are authenticated by providing credentials, and a JWT token is stored in local storage upon successful authentication. Protected routes are guarded by checking for the presence of a valid JWT token.

## Redux Integration

The application integrates Redux for state management. Redux is used to manage user authentication state and handle actions such as logging in and logging out.

## Service Worker (Optional)

The application includes an optional service worker for enabling offline capabilities and faster loading. Service worker registration is handled in the `index.js` file.

