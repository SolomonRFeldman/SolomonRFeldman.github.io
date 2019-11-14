---
layout: post
title:      "Javascript Project"
date:       2019-11-14 10:16:36 +0000
permalink:  javascript_project
---


For my javascript project I was tasked with making a single page application with a javascript front end and a rails api backend. For my idea, I thought of singe page applications I had used, and a lot of them tended to be character planners for videogames. The one game I played that was missing one made by the community was Crusader Kings II. In the game you are able to design your ruler that you start off with, but if you leave the menu, you lose your character, there is no persisting them. So I set about making a single page application that would allow you to create a character and save it to the database for reuse some other time.

My process for creating the app was starting off with the front end. I would create one component to a character, have the javascript mostly finished for that component, and then move to the back end to allow my js to post/get the data it was designed to get, then repeat the cycle. Most all of my data was put on the backend in order to preserve having one source of truth, although a drawback to this is that sometimes elements take a little bit to load waiting on async requests.

One issue I would run into consistanly during this project was properly object orienting my front end. Trying to object orient javascript functionality felt aimless compared to what I was used to in ruby. So many JS classes had intertwining functionalities it was hard to decide what went where, and with no framework like rails, there was no set in stone structure.

However all in all, I came back from this project extremely excited. When I run it up and use it, I feel like I finally built a 'real' website.
