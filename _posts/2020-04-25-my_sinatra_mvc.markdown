---
layout: post
title:      "My Sinatra MVC****"
date:       2020-04-25 07:24:42 +0000
permalink:  my_sinatra_mvc
---


My sinatra MVC project is a small todo app in which it requires the user to sign in and then login. Afterwards, the user is taken to a tasklist. The task itself consists of two options, a name and content. A user can add, edit and delete a task. As the user adds a task, the task adds itself back into the list. At that point the task can then be given the choice to be edited, or deleted, as well as another option to add another task. The task list, adding, editing and deleting options are only available to a user that has signed up with a unique username and email.

The models of which I had used were a User class and Task class. A User class has many tasks and has a secure password, while a task belongs to a User. I used these two models as integral parts in order for my MVC to work. My controller has an Application controller in which is the main controller to run my application. It houses the helpers, which are integrated implicit methods for user authentification in order to make views easier to read. It also houses the home route by "/". The User controller is inherited by the Application controller, I had used the User controller to be the controller in which works with user login, logout and signup features. The Tasks controller is where i keep my substance, I used that controller to build out the routes and paths through my views in order to build my tasklist, and edit/update and delete functionality. I had kept the layout simple to use, in which there are only forms placed for each of my views. 
