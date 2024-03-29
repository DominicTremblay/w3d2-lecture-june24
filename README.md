# W7D3 - Lecture - CRUD with Express

### What is Express?

- Express is a Web framework for NodeJS
  - Routing
  - Layer on top of node HTTP server
  - Middleware
  - Template Engine(ejs)

## Resources

Resources for our movie quotes App

- quotes
- comments

## CRUD Operation

For each resource, we want to:

- create => creating a new resource
- read => getting a resource
- update => changing a resource
- delete => deleting a resource

### http methods

What language does a client use to makes request to the server ? http

http protocol gives us verbs

- Create => Create a new ressource => Post
- Read => Get a resource => Get
- Update => Change a resource => Put
- Delete => Delete a resource => Delete

### Scoping information

- collections vs single entity
- which one?

### End Points

We design design the following end points for our quotes app:

| Action                                | http verb | end point                |
| ------------------------------------- | --------- | ------------------------ |
| List all quotes                       | GET       | get '/quotes'            |
| Get a specific quote                  | GET       | get '/quotes/:id'        |
| Display the new form                  | GET       | get '/quotes/new         |
| Create a new quote                    | POST      | post '/quotes            |
| Display the form for updating a quote | GET       | get '/quotes/:id/update' |
| Update the quotes                     | PUT       | put '/quotes/:id         |
| Deleting a specific quote             | DELETE    | delete '/quotes:id'      |

#### Nested Resources

You may need to access a nested resources. For example, you need to create a new comment.

| Action               | http verb | end point                  |
| -------------------- | --------- | -------------------------- |
| Create a new comment | POST      | post '/quotes/:id/comments |

## Demo

We created a movie quotes app demonstrating the use of Express with RESTful routes.

### To run the app

- npm install
- node server.js
