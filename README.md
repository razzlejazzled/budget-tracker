# budget-tracker
For this app, I was provided with some starter code, and was asked to build a budget tracker that was able to serve as a progressive web application. Much of the base app came pre-built, and the bulk of my task was converting the app into a PWA. 

# starter code
The following files were provided as starter code:
* /models/transaction.js
* /public/icons (all)
* /public/index.html
* /public/index.js
* /public/styles.css
* /routes.api.js
* package.json
* server.js

The following changes were made to the starter code
* /public/index.html
    * added a link to /public/manifest.webmanifest
    * added script tag and code for the service worker
    * added a script tag for db.js
* server.js
    * line 6 was changed to include process.env.PORT to allow for Heroku deployment

# dependencies
This app is built with compression, express, lite-server, mongoose, and morgan.

## User Story
AS AN avid traveller
I WANT to be able to track my withdrawals and deposits with or without a data/internet connection
SO THAT my account balance is accurate when I am traveling

## Business Context

Giving users a fast and easy way to track their money is important, but allowing them to access that information anytime is even more important. Having offline functionality is paramount to our applications success.


## Acceptance Criteria
GIVEN a user is on Budget App without an internet connection
WHEN the user inputs a withdrawal or deposit
THEN that will be shown on the page, and added to their transaction history when their connection is back online.
