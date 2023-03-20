# Auth API
To run this api on your machine, you have to install nodejs and npm installed. You can check here on how to install nodejs
- go ahead to clone the repository or download the zipped file
- open the project directory in your preferred code editor
- then open a new terminal and run "npm install". This installs the projects dependencies
- after a successful installation, run "npm start" in your terminal to start the server which is hosted on port 4000
- once the server is started, go to http:localhost:4000. To be able to interact with the API, use postman to send requests to the following routes.
- POST http://localhost:4000/api/v1 - Signup route
  send a post request with a json populating with the following details to sign up 
  {
    "firstname": '',
    "lastname": "",
    "email": "",
    "phoneNum": "",
    "password": ""
  }

- POST http://localhost:4000/api/v1/login - Login route
  Send a post request with your registered email and password as json to the route above to login through the api.
- GET http://localhost:4000/api/v1/refresh this route is used to get an access token while the refresh token is still valid

- GET http://localhost:4000/api/v1/logout Logout route
  This routes logs out a user
  Note that mongodb is used for this api... You can download mongo on your pc or use the web version.
  
  ### Enironment variables
  Create a .env file in the root directory and populate it accordingly
  
  MONGO_URI
  
  ACCESS_TOKEN_SECRET
  
  REFRESH_TOKEN_SECRET
