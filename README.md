
# CRUD REST API

CRUD is a common abbreviation when it comes to getting started with any framework or programming language. CRUD basically stands for Create, Read, Update and Delete. These are operations that can be performed on resources in your application. Go is not opinionated on how to create these CRUD applications, and therefore it is up to the developer to decide what he/she wants to work with.

In this project, I learnt how to develop a simple CRUD application that uses Go Gin framework to route HTTP requests to handlers that correspond to the CRUD operations. I have used the PostgreSQL database as our datastore. Beside that,I have used a developer friendly ORM called Gorm.

I have build a book API that allows users to perform all the CRUD operations.


## Application structure

The application structure that we will use is quite simple. It is made of two modules namely:

**database module**: For all database related operations such as connection to the database.

**controller module**: For CRUD operations.
At the root level we will have the main.go file that will host code for initializing the database, and HTTP routing and running the server.
## Database setup

It is a good idea to start with the database setup and the resources that we are going to perform the CRUD operations on. In order to communicate with the database, we need to create a database client that we will use to call Create, Update, Find and Delete methods against the database. This database client will be exported and used in other parts of our code like in the controller module.

In the database module, created a **postgres.go** file.
## Configure CRUD Operation on the Controller

**controllers/gin.go**

This file hosts all the code for the CRUD operations. These handler functions route HTTP requests from the client and perform database operations accordingly.
## Testing CRUD REST API Operation

**Create a book:**

![image](https://github.com/ritiktyagi1/go-crud-api/assets/54032937/686fde73-fe9b-431b-a5b3-2e6b45f3a3bb)


**Get a book:**

![image](https://github.com/ritiktyagi1/go-crud-api/assets/54032937/d689f625-50d5-47dd-be75-50bab49ba525)


**update a book:**

![image](https://github.com/ritiktyagi1/go-crud-api/assets/54032937/04f31109-b28b-41d2-bede-af8ed6717c38)


**Get all books:**

![image](https://github.com/ritiktyagi1/go-crud-api/assets/54032937/7bbdace5-47e7-4593-8005-46e89d3c2f6a)


**Delete a book:**

![image](https://github.com/ritiktyagi1/go-crud-api/assets/54032937/c6a2efed-f35e-4150-85ff-8013304ab2d6)


## Tech Stack

**Language:** Go 

**Web framework:** Gin

**Library:** GORM

**DB:** PostgreSql

**Testing tool:** Insomnia

