# what2watch
android app - rank, filter and sort movies and TV shows you want to watch. Developed using Ionic2/Cordova/Angular 

## Demo
For an active demo please visit **TODO - add heroku link**

This app was developed as a proof of concept. While functional, it is still in development and has not been thoroughly tested for security. Therefore please use throwaway login/password info while testing. Do not reuse important login credentials from gmail/facebook, banking sites, etc.

##User Overview
what2watch is an application developed for use on mobile android devices used to bring together all of your watch lists across different services into one place and help you decide once and for all what you want to watch

You can display lists with the ability to filter source of the content (netflix, hbo, hulu, physical disk, computer, etc), type (movie, TV show), or genre. You may also group and sort the results based on date added, rank, alphabetical, etc. You may also search your list to view details on any item that may help you make a decision on what to watch.

Once you have viewed an item you may archive it for future reference.

###How it works

##Developer Notes

###Release history/Change Log
01/07/16 - Development started

###API Integration


###Future Development

##Build details
1. If you would like to build for mobile platforms you will need to install ionic and cordova globally.

##How to build and deploy yourself

This app utilizes MongoDB. You can either use a local database or a cloud deployment such as MongoLab. Mongo must be installed and running if you are using local.

###Setup Instructions
1. Clone this repository ```git clone https://github.com/preetgujral/what2watch.git```
2. Change into the directory ```cd what2watch```
3. Add package dependencies using ```npm install```
4. Set local environmental variables:
  1. in root directory create a file called '.env'


5. Connect to database:
  1. Local mongo database
    1. open the config.js file and replace '/pet_app' with the database you would like to use
  2.  Mongolabs database
    1. add following line to your .env file, replacing dbuser, dbpassword, host, port, and dbname with the appropriate information
    2. ```MONGOLAB_URI='mongodb://dbuser:dbpassword@host:port/dbname'```
    3. if database is connected through heroku check https://devcenter.heroku.com/articles/mongolab#getting-your-connection-uri.
    4. if connected through mongolab directly navigate to https://mongolab.com/databases/yourDBNamehere
  6. You can then run the application locally using ```npm start``` and navigating to 'localhost:YourChosenPort'.

###Code Style and Directory Structire
1. JSCS is used as the style and linting tool to maintain a common coding convention. Custom settings are included in .jscsrc in the root directory

2. The repo has the following directory structure. Not all files are shown in the individual directories. Self Explanatory configuration files in the root directory are also seletively listed. hooks, node_modules, www/lib are system folders and should not be modified without knowledge of how they work.
