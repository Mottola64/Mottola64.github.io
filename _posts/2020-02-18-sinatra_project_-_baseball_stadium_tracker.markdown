---
layout: post
title:      "Sinatra Project - Baseball Stadium Tracker"
date:       2020-02-18 22:05:40 -0500
permalink:  sinatra_project_-_baseball_stadium_tracker
---


Baseball is America's Favorite past time and being that each team's stadium is unique, I plan on visiting all of them. Traveling to and visiting 30 stadiums can be a huge undertaking and frankly it could be hard to keep track of which stadiums you've visited if you don't write them down. This is how I came up with the idea to build a Baseball Stadium Tracker.

My Baseball Stadium Tracker is built in Sinatra using the MVC design pattern. The Model View Controller (MVC) design pattern provides a separation of concerns where each part of the application has its own purpose and interacts with the other parts of the application.

The Model is where the data is saved and manipulated, it is the logic portion of an application. In Sinatra, models are typically Ruby classes, and can connect to databases to save data. Views is the front-end portion of an application and are the only part of a web application that a user would interact with. In Sinatra, views are created using .erb files and consist of HTML and embedded Ruby. Controllers are the go-between for models and views. Controllers relay data from the browser to the application and back. Controllers consist of routes that take requests from the browser, run code using the models, and render an .erb file for the users to see.

For my project, a user can make a login, and once they are logged in they can fill out a form to add a new baseball stadium that they've visited. They will then be shown a list of stadiums that they've visited and if they notice a mistake or if a stadium name changed, they can edit the team and stadium name. If for some reason they added a stadium by mistake they could also delete it from their list.

In the future I could add functionality where you can add friends on the app and see which stadiums they've visited, and if you both haven't visited a specific baseball stadium yet, you could plan a trip together!
