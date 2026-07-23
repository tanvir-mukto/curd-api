# curd-api
# To-Do List CRUD API

This is a small, in-memory RESTful API built for managing a simple To-Do list. It supports full CRUD operations (Create, Read, Update, Delete) and uses proper HTTP status codes.

## 🚀 How to Install and Run

1. Clone the repository:
   `git clone [your-repo-link]`
2. Install dependencies (if using Node/Express) or set up env (if using Python/FastAPI).
3. Start the server:
   `npm start` OR `uvicorn main:app --reload` (change based on your stack)
   
The server will run on `http://localhost:3000` (Express) or `8000` (FastAPI).

## 🚏 API Endpoints

| CRUD Operation | HTTP Method | Endpoint | Description |
| :--- | :--- | :--- | :--- |
| **Read (All)** | `GET` | `/tasks` | Returns all tasks |
| **Read (Single)** | `GET` | `/tasks/{id}` | Returns a single task by ID |
| **Create** | `POST` | `/tasks` | Creates a new task (requires JSON body) |
| **Update** | `PUT` | `/tasks/{id}` | Updates a task by ID |
| **Delete** | `DELETE` | `/tasks/{id}` | Removes a task by ID |

## 🧪 Sample Request (cURL)
```bash
curl -i -X POST http://localhost:3000/tasks \
-H "Content-Type: application/json" \
-d '{"title":"Buy milk"}'
