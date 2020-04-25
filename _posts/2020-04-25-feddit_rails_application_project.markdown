---
layout: post
title:      "Feddit Rails Application Project"
date:       2020-04-25 07:38:17 +0000
permalink:  feddit_rails_application_project
---


Hi, this is Azraf Chowdhury. I am here today, discussing my application that I had built with ruby on rails. The application is called Feddit. I challenged myself to build a light clone of reddit. 

My application consists of 4 models. 

1. User
2. Subfed
3. Post
4. Comment

I had built my application from scratch. I had first started building out the databases and activerecord associations for my rails application. My post model acts as my join table between a user and subfed. 

My user model requires a username, email and password. My user model also contains nested params, which are displayed on The user index page as a user name card. The nested params are bio, age and location. A user can create subfeeds, which are categories that house a collection of posts belonging to its category. Users can also build their own posts, edit, update and delete. Users can also create comments belong to specific posts.

Subfeed are different categories or subforums created by the user. An example would be baked goods. Its general and ambiguous but through depth and detail of posts, it can become very descriptive in a manner of speaking. Subfeeds contain a title and description.

Posts are the details that make up the insides of subfeeds. They can add or subtract content and depth from a subfeed. Posts consists of a title and summary, as well as a collection select in which subfed the post belongs to. 

Comments are what get added to posts. they are defined by its user, and belong to a single post. 

That is my project application in a nutshell!

