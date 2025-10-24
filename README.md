# Books REST API - Node.js and Express

## Objective

Create a simple REST API using Node.js and Express.js to perform CRUD operations (Create, Read, Update, Delete) on a list of books stored in memory.

## Key Concepts

* REST API principles
* Express.js routing
* HTTP methods: GET, POST, PUT, DELETE
* JSON handling
* Middleware
* CRUD operations

## Tools and Technologies

* Node.js
* Express.js
* Postman (for testing)
* VS Code

## Setup Instructions

1. Initialize project:

   ```bash
   npm init -y
   ```

2. Install dependencies:

   ```bash
   npm install express
   ```

3. Run the server:

   ```bash
   node server.js
   ```

4. Server runs on:

   ```
   http://localhost:3000
   ```

## API Endpoints

| Method | Endpoint   | Description    | Example Body                                      |
| ------ | ---------- | -------------- | ------------------------------------------------- |
| GET    | /books     | Get all books  | —                                                 |
| POST   | /books     | Add a new book | { "title": "Deep Work", "author": "Cal Newport" } |
| PUT    | /books/:id | Update a book  | { "title": "Updated Title" }                      |
| DELETE | /books/:id | Delete a book  | —                                                 |

## Example Responses

**GET /books**

```json
[
  { "id": 1, "title": "The Alchemist", "author": "Paulo Coelho" },
  { "id": 2, "title": "Atomic Habits", "author": "James Clear" }
]
```

**POST /books**

```json
{ "id": 3, "title": "Deep Work", "author": "Cal Newport" }
```

**DELETE /books/1**

```json
{ "message": "Book deleted successfully" }
```
