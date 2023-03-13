# DublinBusGroupProject

<img src = "https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNTQyNmI1YmRhNmVkZjBhOTkzYjZmYzUyY2MyNThiNWU2ZWNkMjFlMiZjdD1n/e5bNjlMCcfv0cSzlS5/giphy.gif"
 width="700" height="400" />
 
 ## Background

This project was completed in part fulfillment of the UCD Msc in Computer Science. The goal was to improve upon  exisiting Dublin Bus Real-Time applications. This is a single page application that is compatible with both mobile and desktop devices. Minimalism was the goal in order for the site to be easily navigable for users. Data models were created by the team to predict bus journey length times as required by the user. 

note: Both the EC2 and UCD servers initially used to host the website and databases have been switched off. 

### Features

##### Journey 

The core website feature. Users select a start and endpoint along with a departure time. The website will then return a list of suggested ways of completing the journey ordered from quickest to slowest. This includes the number of bus transfers possibly needed and walking distance between stops. 

##### Login

A registration and login service is available py clicking the top left panel, upon registration users can store favourite routes and stops. 

##### Routes

Viewers can search for individual bus routes, for which upon selection a list of stops served by the route will appear both on the side panel and map. Users can select stops to view scheduled departure times.

##### Stops

Users can search for stops and their preferred departure time to find scheduled departures for various routes around that time. If user does not select a time it defaults to current. 

<img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExYzhhZjhjZTRjYjdlNDc2OTZjNzhkMTI3ZTBhYTdmZjczN2M5YWFlMiZjdD1n/Vme1OPBENsJkQmQzGy/giphy.gif" height="600" width="330" />
 
 
 ***ORIGINAL REPO REF: https://github.com/kevinobrien97/comp47360_SummerGroupProject ***
 
 
# ShuttleUp Installation Guide 

Clone repo and run the following:

##### virtualenv envname
##### source envname/bin/activate 

##### pip install -r requirements.txt
##### pip install django-cors-headers

### cd client

##### npm install

##### npm start 

Store your personal Google Maps API key in the env folder and ensure you have enabled access to GoogleMaps' Javascript, Directions and Places APIs. 

## For other keys: 

##### export SQLPW="password-to-shuttleup-DB" 
##### export API="your-openweather-api-key"
##### export django_key="your-own-secret-django-key"

In a second terminal you can optionally do the following: 

##### python manage.py runserver 

this will start Django. To use a local version of our backend you will need to replace our deployed backend IP address to "127.0.0.1", by commenting back in the lines with this IP (and removing the lines with the deployed version). 

