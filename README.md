# Full Stack Burgers BurgerLogger (Node Express Handlebars)

## Overview

A full-stack app that uses the following technologies:

* MySQL
* NodeJS
* Express
* Handlebars.js, &
* A DIY Object-Relational-Mapper / ORM

Follows an MVC design paradigm, using Node and MySQL to query and route data in the app, and Handlebars to dynamically generate HTML.

The live site can be viewed here: https://burgerstack.herokuapp.com/

Heroku Deployment: MySQL JAWSDB server

## Functionality

Burger Stack is a restaurant app that lets users input the names of burgers they'd like to eat. Whenever a user submits a burger's name, the app displays the burger on the left side of the page -- waiting to be devoured. Each burger in the waiting area has a `Eat Me!` button. When the user clicks it, the burger will move to the right side of the page.

The app stores every burger in a MySQL database that is persisted, along with their 'devoured' status.

## Model-View-Controller / MVC Paradigm

Burger Stack is a modular application that utilizes the MVC architectural pattern to structure the codebase into distinct separation of concerns. 

The Model data layer of the application utilizes MySQL to create a persistent database and an Object Relational Mapper (ORM) to retrieve data from the database.

The HTML is dynamically generated using the Handlebars.js template engine, separating the concern of client-side rendering from other aspects of the application for the View layer in the MVC framework.

And finally, Express.js is used as Controllers to handle inputs from the user, to interact with the Model for CRUD operations, and to return query results to the View, separating client-side from server-side routes. 

#### Directory structure

All the recommended files and directories from the steps above should look like the following structure:

```
.
├── config
│   ├── connection.js
│   └── orm.js
│ 
├── controllers
│   └── burgers_controller.js
│
├── db
│   ├── schema.sql
│   └── seeds.sql
│
├── models
│   └── burger.js
│ 
├── node_modules
│ 
├── package.json
│
├── public
│   └── assets
│       ├── css
│       │   └── burger_style.css
│       └── img
│           └── burger.png
│   
│
├── server.js
│
└── views
    ├── index.handlebars
    └── layouts
        └── main.handlebars
```
![screenshot](demo.png
