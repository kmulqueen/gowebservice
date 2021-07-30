# gowebservice

# About
This is a simple REST API that has CRUD functionality built using [GoLang](https://golang.org/). Interacting with this API allows you to create, read, update, and delete fictional users. This API is not attached to a database, so the data is not persistent. The amount of users initialized is 0 so you will need to create users to fully interact.

# Run
To run, make sure you have [Go](https://golang.org/) installed on your machine. Then download the repository file and navigate to the root folder of this repository using your terminal. Once at the root directory of this repo, enter the following command in your terminal

`go run .` 

This will start a web server on `http://localhost:3000`

To interact with the API use a tool like [Postman](https://www.postman.com/) to make requests to the server.

# Paths

 The valid paths for this API are **/users** or **/users/{id}**

# Methods

The available HTTP methods for **/users** are **GET** & **POST**.
- **GET** retrieves all of the existing users
- **POST** creates a new user
  - Example Body (JSON): `{"FirstName": "Foo", "LastName": "Bar}`

The available HTTP methods for **/users/{id}** are **GET**, **PUT**, **DELETE**.
- **GET** retrieves a user by their ID
- **PUT** updates a user by their ID
    - Example Body (JSON): `{"ID": 1, "FirstName": "Sally", "LastName": "Smith"}`
- **DELETE** deletes a user by their ID
