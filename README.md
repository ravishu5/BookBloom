# BookBloom

## Introduction
BookBloom is a backend service designed to manage a collection of books. It offers a simple yet powerful API to retrieve all books, add a new book, and update book details.

## Features
- **Retrieve All Books**: (get) https://book-bloom.vercel.app/api/books/
- **Add Book**: (post) https://book-bloom.vercel.app/api/books/
- **Update Book**: (put) book-bloom.vercel.app/:id  

### Prerequisites
What things you need to install the software and how to install them:

- Node.js
- MongoDB
- npm (Node Package Manager)

### Installing
A step-by-step series of examples that tell you how to get a development environment running.

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/BookBloom.git
2. **Navigate to the project directory:**
   ```bash
   cd BookBloom
3. **Install dependencies:**
   npm install
4. **Start the server:**
   node index.js

## API Endpoints

### Retrieve All Books
- **URL**
  - `/books`
- **Method:**
  - `GET`
- **Description**
  - Retrieves a list of all books in the collection.

### Add Book
- **URL**
  - `/books`
- **Method:**
  - `POST`
- **Body** *(example)*:
  ```json
  {
    "title": "Example Book Title",
    "author": "Author Name",
    "genre": ["Fiction", "Adventure"],
    "isbn": "123-4567890123"
  }

### Update Book

- **URL**
  - `/books/:id`

- **Method:**
  - `PUT`

- **URL Params**
  - Required: `id=[string]` (ID of the book to update)

- **Body** *(example)*:
  ```json
  {
    "title": "Updated Book Title",
    "author": "Updated Author Name",
    "genre": ["Mystery", "Thriller"],
    "isbn": "987-6543210987"
  }

