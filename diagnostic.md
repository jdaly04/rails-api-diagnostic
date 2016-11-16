# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash
A back-end exists to store, retrieve, receive data. Keeps stuff secure,
allows user authentication. Allows front-end to work. 
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
model
```

Which layer in the MVC pattern communicates with the model?

```bash
The controller.
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
We use JSON instead.
```

What does C.R.U.D stand for?

```bash
Create, Read, Update, Delete.
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```bash
index, create, show, update, destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
Browser communicates with the routes layer, which makes a decision on which
controller to pass the request to. Controller then goes to the model and tells
it to retrieve the data in ":id1" from the people database. Model does that,
gives it back to the controller, back to the server, and then to the Browser
with the status code / appropriate response.
```

What is the command to generate a new rails-api app?

```bash
rails new my_api --api
```

What is the command to start an instance of a rails server?

```bash
bundle exec rails server
```

What are the commands to drop, create and migrate a database from the command
line? (3 bullet points)

```bash
bundle exec rake db:drop
bundle exec rake db:create
bundle exec rake db:migrate
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bundle exec generate scaffold pet name:string age:integer
```
