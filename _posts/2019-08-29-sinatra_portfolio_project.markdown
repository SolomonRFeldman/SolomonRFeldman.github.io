---
layout: post
title:      "Sinatra Portfolio Project"
date:       2019-08-29 17:55:37 +0000
permalink:  sinatra_portfolio_project
---


My second project for the full stack web development program was to make a web app using sinatra. I chose to make an app where users would be able to list the games they've played and make posts about them. I began with mapping the relationships by creating a schema and controllers to go with it. Then I built the functionality for users to create a user and login. I decided I wanted to have users be able to say they've played a game, post about a game, and rate the game. Each would be able to be done in one form and all the infomation in that form would have to be displayed as one element, this is where I discovered the beauty of sql queries. In order to show that information I would have had to iterate through a users posts and searching the database for the relation on each iteration. To avoid this and make it so I only hit the database once to show the feed I used an sql query to aggrigate all the data into one object. On completing the post form it would tie the rating, post, and if you just played the game, together through relational mapping, and the query would take that data and join the tables with the relevent information. After I made sure my database had all the information and validations I wanted I went about creating the controllers and views. Once that was done, I finally stylized my website with bootstrap.
