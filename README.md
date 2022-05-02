# DownToMeet-MERN

Down To Meet: An event management website built using React, Express, Node.js, MongoDB Atlas, AWS S3, API hosted on Heroku.
### Table of Content for README.md
1) Steps to make this project work
2) Features
3) Screenshots


### Steps for making this project work:
1) clone this repo using 
```
    git clone https://github.com/deep77patel/DownToMeet.git
```
2) open cmd with pwd ./DownToMeet-MERN and type 
```"npm install"``` this will create npm  modules and package-lock.json
3) create .env file with content like<br>
```
  mongo_DB_Connection = mongodb+srv://<username>:<password>@cluster0.himhp.mongodb.net/<dbname>?retryWrites=true&w=majority
  ACCESS_KEY_ID = "Provided through AWS S3"
  SECRET_ACCESS_KEY = "Provided through AWS S3"
  
```
4) Type ```npm run dev``` or ```nodemon backend/server```,this will make the express server run at localhost:8000
5) For frontend to work follow these steps
```
cd client
npm install
``` 
6) Type ```npm run dev``` or ```npm start```,this will make the react app start at localhost:3000

### Features:
1) Password hashing during register/login for security using npm package "bcrypt"
2) Using tokens and verifying for protecting routes using npm package "jsonwebtoken"
3) Creating events with proper validations
4) Storing images on AWS S3 and using timestamp for unique identification of image using npm package "multer"
5) Displaying events ascendingly sorted with base of Date
6) Filtering events based on event-type(seminar/webinar/workshop and Your events)
7) Deleting events that you have created.
8) Requesting registration for event as an attendee.
9) Accepting/Rejecting participant request as an organizer of event.
10) Viewing number of participants and all details of participants.
