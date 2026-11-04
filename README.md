Name: Bolla Pradhyumna

# 📚 Books REST API

A RESTful API built using **Node.js, Express.js, and SQLite** to manage book records. This project demonstrates CRUD operations (Create, Read, Update, and Delete) and REST API development.

## 🚀 Technologies Used

- Node.js
- Express.js
- SQLite
- JavaScript
- Postman
- Git & GitHub

## ✨ Features

- Create new book records.
- Retrieve all books.
- Retrieve a specific book using its ID.
- Search books by title.
- Sort books in ascending or descending order.
- Filter books by price range.
- Apply pagination using limit and offset.
- Update existing book details.
- Delete book records.
- Validate request data and handle errors.

## 📁 Project Structure

```text
Pradhyumna_Lab_3/
│
├── app.js
├── db.js
├── package.json
├── package-lock.json
├── .env
├── .gitignore
└── books.db
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/bollapradhyumna1409-collab/Pradhyumna_Lab_3.git
```

### 2. Navigate to the Project Folder

```bash
cd Pradhyumna_Lab_3
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Configure Environment Variables

Create a `.env` file:

```env
PORT=3000
```

### 5. Start the Server

```bash
npm start
```

The API will run at:

```text
http://localhost:3000
```

## 🔗 API Endpoints

| HTTP Method | Endpoint | Description |
|---|---|---|
| GET | `/books` | Get all books |
| GET | `/books/:id` | Get a book by ID |
| POST | `/books` | Add a new book |
| PUT | `/books/:id` | Update a book |
| DELETE | `/books/:id` | Delete a book |

## 🔍 Query Parameters

The GET `/books` endpoint supports:

| Parameter | Description |
|---|---|
| `search_q` | Search books by title |
| `order_by` | Sort field |
| `order` | ASC or DESC |
| `limit` | Maximum number of records |
| `offset` | Number of records to skip |
| `min_price` | Minimum book price |
| `max_price` | Maximum book price |

Example:

```text
GET /books?search_q=Python&order_by=price&order=ASC&limit=5&offset=0
```

## 📝 Sample JSON Request

### POST /books

```json
{
  "title": "Python Programming",
  "author": "John Smith",
  "price": 500
}
```

## 🧪 Testing with Postman

All API endpoints can be tested using Postman.

1. Start the Express server.
2. Enter the API endpoint.
3. Select the appropriate HTTP method.
4. For POST and PUT, select Body → raw → JSON.
5. Send the request and verify the response.

## ⚠️ Error Handling

The API handles:

- Missing required fields.
- Invalid price values.
- Book records not found.
- Invalid routes.
- Database errors.

## 👨‍💻 Author

**Bolla Pradhyumna**

GitHub: https://github.com/bollapradhyumna1409-collab/Pradhyumna_Lab_3.git

## 🎯 Project Objective

To understand REST API development, HTTP methods, Express.js routing, SQLite database operations, request validation, and API testing using Postman.

---

⭐ If you find this project useful, feel free to explore the repository!
