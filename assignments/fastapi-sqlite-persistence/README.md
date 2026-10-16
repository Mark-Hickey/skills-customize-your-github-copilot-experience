# 📘 Assignment: Persisting FastAPI Data with SQLite

## 🎯 Objective

Extend a FastAPI book API to store its data in a SQLite database instead of an in-memory collection. Practice creating a database table and using SQL queries to create, retrieve, update, and delete records.

## 📝 Tasks

### 🛠️ Create the Books Database

#### Description
Set up a SQLite database for the books API so book records are stored between application runs.

#### Requirements
Completed program should:

- Use Python's built-in `sqlite3` module to connect to a database file
- Create a `books` table with an integer primary key, a title, and an author
- Create the table if it does not already exist
- Confirm that the database file and table are created when the application starts


### 🛠️ Connect Read and Create Endpoints

#### Description
Replace the in-memory book collection in the FastAPI application with database queries for listing, retrieving, and creating books.

#### Requirements
Completed program should:

- Update `GET /books` to return all books stored in the database
- Update `GET /books/{book_id}` to return the matching book or an HTTP 404 response if it does not exist
- Update `POST /books` to insert a book, save the change, and return its generated ID
- Use parameterized SQL queries for values supplied by API requests


### 🛠️ Persist Updates and Deletions

#### Description
Update the remaining book endpoints to modify and remove database records, then verify that the API uses persistent data.

#### Requirements
Completed program should:

- Update `PUT /books/{book_id}` to save a book's new title and author to the database
- Update `DELETE /books/{book_id}` to remove the book from the database
- Return an HTTP 404 response when an update or delete request uses an unknown book ID
- Verify that newly created or updated books remain available after restarting the application
