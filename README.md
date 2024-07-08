# MovieHunt

MovieHunt is a backend application for a movie review app. It is built using Java and provides APIs for users to review movies, fetch movie details, and more.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)

## Features
- User authentication and authorization
- CRUD operations for movie reviews
- Fetch movie details
- Rate movies
- Comment on reviews

## Installation

### Prerequisites
- Java 11 or higher
- Maven
- Git

### Steps
1. Clone the repository
    ```bash
    git clone https://github.com/Rizz-33/MovieHunt.git
    cd MovieHunt
    ```

2. Build the project
    ```bash
    mvn clean install
    ```

3. Run the application
    ```bash
    mvn spring-boot:run
    ```

## Usage
Once the application is running, you can access the API at `http://localhost:8080`.

### Example Requests

- **Fetch all movies**
    ```bash
    GET /api/movies
    ```

- **Add a new review**
    ```bash
    POST /api/reviews
    Content-Type: application/json

    {
        "movieId": 1,
        "userId": 1,
        "rating": 5,
        "comment": "Great movie!"
    }
    ```

## API Endpoints

### Movies
- `GET /api/movies` - Fetch all movies
- `GET /api/movies/{id}` - Fetch movie by ID
- `POST /api/movies` - Add a new movie
- `PUT /api/movies/{id}` - Update a movie
- `DELETE /api/movies/{id}` - Delete a movie

### Reviews
- `GET /api/reviews` - Fetch all reviews
- `GET /api/reviews/{id}` - Fetch review by ID
- `POST /api/reviews` - Add a new review
- `PUT /api/reviews/{id}` - Update a review
- `DELETE /api/reviews/{id}` - Delete a review

### Users
- `GET /api/users` - Fetch all users
- `GET /api/users/{id}` - Fetch user by ID
- `POST /api/users` - Add a new user
- `PUT /api/users/{id}` - Update a user
- `DELETE /api/users/{id}` - Delete a user

## Contributing
1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Create a new Pull Request
