# Movies API

A RESTful Movie Review API built with **Spring Boot**. It allows users to fetch movie data and submit/read reviews. Designed as a backend service for movie-based applications.



##  Features

*  Manage a collection of movies
*  Submit and retrieve reviews for each movie
*  Uses Spring Boot with MVC architecture
*  Connects to a database using Spring Data JPA



##  Technologies Used

* Java 17
* Spring Boot
* Spring Web
* Spring Data JPA
* MongoDB
* Maven



##  Project Structure

```
movies-api
├── .idea/
├── movies/
│   ├── pom.xml               # Maven project file
│   ├── mvnw, mvnw.cmd        # Maven wrappers
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/dev/hk/movies/
│   │   │   │   ├── Movie.java
│   │   │   │   ├── Review.java
│   │   │   │   ├── MovieController.java
│   │   │   │   ├── ReviewController.java
│   │   │   │   ├── MovieService.java
│   │   │   │   ├── ReviewService.java
│   │   │   │   ├── MovieRepository.java
│   │   │   │   ├── ReviewRepository.java
│   │   │   │   └── MoviesApplication.java
│   │   └── resources/
│   │       ├── application.properties
│   │       ├── .env
│   │       └── .env.examples
│   └── test/java/dev/hk/movies/MoviesApplicationTests.java
```



##  Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/movies-api.git
cd movies-api/repos/movies
```

### 2. Configure the environment

Set your environment variables in `src/main/resources/.env` or use `application.properties` for DB configs.

### 3. Run the app

Using Maven Wrapper:

```bash
./mvnw spring-boot:run
```

Or with installed Maven:

```bash
mvn spring-boot:run
```

### 4. Access Endpoints

Default: `http://localhost:8080`

Example endpoints:

* `GET /api/movies` – fetch all movies
* `GET /api/movies/{id}` – fetch single movie by ID
* `POST /api/reviews` – add a review
* `GET /api/reviews/{movieId}` – get reviews for a movie



##  Testing

Run tests using Maven:

```bash
mvn test
```



##  Author

Harkishan Solanki



##  License

This project is licensed under the MIT License.
