# API Documentation

This document outlines the endpoints available in the Flask API along with their functionalities and supported HTTP methods.

## Base URL

The base URL for all endpoints in this API is `http://localhost:5000/` when running locally.

---

## User Routes

### GET `/users`

- **Description:** Retrieves a list of all users.
- **Method:** GET
- **Response Format:** JSON
- **Response Code:** 200 (Success)

### POST `/users`

- **Description:** Creates a new user.
- **Method:** POST
- **Request Format:** JSON
    ```json
    {
        "username": "string",
        "password": "string",
        "email": "string",
        "role_id": "integer"
    }
    ```
- **Response Format:** JSON
- **Response Code:** 201 (Created)

---

## Book Routes

### GET `/books`

- **Description:** Retrieves a list of all books.
- **Method:** GET
- **Response Format:** JSON
- **Response Code:** 200 (Success)

### POST `/books`

- **Description:** Adds a new book to the database.
- **Method:** POST
- **Request Format:** JSON
    ```json
    {
        "book_number": "string",
        "book_name": "string",
        "publication_year": "integer",
        "pages": "integer",
        "category_id": "integer"
    }
    ```
- **Response Format:** JSON
- **Response Code:** 201 (Created)

---

## Wishlist Routes

### GET `/wishlists`

- **Description:** Retrieves a list of all wishlists.
- **Method:** GET
- **Response Format:** JSON
- **Response Code:** 200 (Success)

### POST `/wishlists`

- **Description:** Adds a book to a user's wishlist.
- **Method:** POST
- **Request Format:** JSON
    ```json
    {
        "user_id": "integer",
        "book_id": "integer"
    }
    ```
- **Response Format:** JSON
- **Response Code:** 201 (Created)

---

## Rating Routes

### GET `/ratings`

- **Description:** Retrieves a list of all ratings.
- **Method:** GET
- **Response Format:** JSON
- **Response Code:** 200 (Success)

### POST `/ratings`

- **Description:** Adds a rating and review for a book.
- **Method:** POST
- **Request Format:** JSON
    ```json
    {
        "user_id": "integer",
        "book_id": "integer",
        "rating": "float",
        "review": "string"
    }
    ```
- **Response Format:** JSON
- **Response Code:** 201 (Created)

---

**Note:** Replace `"string"`, `"integer"`, and `"float"` with actual string, integer, and float values respectively when making requests to the API.
