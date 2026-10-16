# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a REST API with FastAPI to manage a collection of books. Practice defining endpoints, validating request data, and using HTTP methods and status codes to create, retrieve, update, and delete resources.

## 📝 Tasks

### 🛠️ Create the FastAPI App and Read Endpoints

#### Description
Create a FastAPI application that stores a small collection of books in memory and lets clients retrieve the collection or an individual book.

#### Requirements
Completed program should:

- Create a FastAPI application and run it locally with Uvicorn
- Define a `Book` with an integer `id`, a `title`, and an `author`
- Implement `GET /books` to return all books and `GET /books/{book_id}` to return a book by ID
- Return an HTTP 404 response when the requested book ID does not exist


### 🛠️ Add Books with a POST Endpoint

#### Description
Allow clients to add books to the collection by sending JSON data to the API.

#### Requirements
Completed program should:

- Define a Pydantic request model requiring a book's `title` and `author`
- Implement `POST /books` to create a book and assign it a unique integer ID
- Return the created book, including its ID, with HTTP status code 201
- Reject requests that omit a required field with FastAPI's validation response


### 🛠️ Update and Delete Books

#### Description
Complete the API's CRUD functionality by allowing clients to update or remove a book by ID.

#### Requirements
Completed program should:

- Implement `PUT /books/{book_id}` to update a book's title and author
- Implement `DELETE /books/{book_id}` to remove a book
- Return an HTTP 404 response when an update or delete request uses an unknown book ID
- Verify the endpoints using the interactive API documentation at `/docs`
