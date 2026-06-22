# Go HTTP API - Articles

This project is a simple Go application that demonstrates how to build a basic HTTP server with routes and JSON responses.

---

## Features

- HTTP server built using Go’s `net/http` package
- Basic homepage endpoint
- Endpoint that returns a list of articles in JSON format
- Simple data structure using Go structs
- JSON encoding with `encoding/json`

---

## Endpoints

### `/`
- **Method:** `GET`
- **Description:** Returns a simple message confirming the server is running

**Response:**
```text
Homepage Endpoint Hit

/articles
Method: GET
Description: Returns a list of articles in JSON format

Example response:

[
  {
    "title": "Test Title",
    "desc": "Test Description",
    "content": "Hello World!"
  }
]
```

# Project Structure
- Article → struct representing an article with:
- title
- description
- content
- Articles → slice of Article
- allArticles() → handler function that returns all articles as JSON
- homePage() → handler for the root endpoint (/)
- handleRequests() → registers routes and starts the HTTP server
- main() → application entry point

# How to Run
```bash
# Clone the repository
git clone https://github.com/your-username/your-repo.git

# Navigate to the project folder
cd go-api

# Run the application
go run main.go
```

# Server

Once running, the API will be available at:

http://localhost:8081

# Technologies Used
Go (Golang)
net/http
encoding/json


# Example Code Behavior

When accessing /articles, the server returns a JSON array of articles defined in memory:
```json
Article{
  Title: "Test Title",
  Desc: "Test Description",
  Content: "Hello World!",
}
```

# Author

Developed by @lmrick  
For learning and portfolio purposes.

# License

This project is open-source and free to use for educational purposes.
