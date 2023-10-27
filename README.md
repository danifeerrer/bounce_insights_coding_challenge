# Country Information App

This is a simple web application that provides information about different countries. It consists of two main components: the backend and the client, which communicate with each other. The client is built using React, and the application is deployed on Heroku.

## Deployment

### Backend Deployment

1. The backend of this application is located in the `backend_country` directory.

2. The backend server is built using Express and provides a set of API endpoints for fetching country information.

3. To deploy the backend to Heroku, follow these steps:

   - Make sure you have the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli) installed.

   - Create a `Procfile` in the root of your `backend_country` directory. The `Procfile` should contain the following line:

     ```
     web: node server.js
     ```

   - Commit your changes if you haven't already.

   - Run the following commands in your terminal:

     ```bash
     heroku login
     heroku create your-backend-app-name
     git push heroku master
     ```

4. Your backend should now be deployed to Heroku. You can access it using the URL provided by Heroku.

### Client Deployment

1. The client of this application is located in the `client_country` directory.

2. The client is built using React.

3. To deploy the client to Heroku, follow these steps:

   - Make sure you have the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli) installed.

   - Commit your changes if you haven't already.

   - Create a `Procfile` in the root of your `client_country` directory. The `Procfile` should contain the following line to start the client application:

     ```
     web: npm run start
     ```

   - Run the following commands in your terminal:

     ```bash
     heroku login
     heroku create your-client-app-name
     git push heroku master
     ```

4. Your client should now be deployed to Heroku. You can access it using the URL provided by Heroku.


## CORS Configuration

This application uses CORS (Cross-Origin Resource Sharing) to enable communication between the backend and the client, even if they are hosted on different domains. The CORS configuration is set up in the backend.

## Usage

1. Access the deployed client application to interact with the country information.

2. The client communicates with the backend to fetch data using Axios.

3. The backend serves data and handles CORS to allow requests from the client application.

4. You can explore information about different countries and make API requests to the backend as needed.

