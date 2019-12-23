---
layout: post
title:      "Serializing Rails API Responses"
date:       2019-12-23 20:22:17 +0000
permalink:  serializing_rails_api_responses
---


Throught my Javascript/React projects, I have used the rails API to interact with the models of my database. The first thing I learned while making an API was that I don't like serializers. Gems that provide serializers take way too much control away from the process of providing the correct data. For example, the first issue I ran into, was that the serializer I was using would have an N+1 query problem if my data was nested where it would ping the database everytime a resource was grabbing data from it's has_one/has_many related model. That in itself made me go down the path of just making custom methods. Through these methods I could directly write my own SQL queries and grab exactly what I needed from the database for that specific call with one ping to the database. This also allows me to organize my data in the way that I want it, forgoing nesting resources and only being able to return one resource, like the .to_json method does to an activerecord object. If you use .to_json together with another resource in a hash, it will double convert to json, turning the .to_json resource into a string. When you write your own methods for your controllers you can return multiple resources as a hash and rails will convert it to json by itself. This combined with the specific syntax to_json requires to grab what you need, which I've found is a pain to deal with, has made me dismiss it in most cases in favor of turning my resource into a hash and using plain old ruby to grab the data I need.
