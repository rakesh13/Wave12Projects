# Movies

## Problem Statement

Build a system to manage Movies.

## Requirements:

1. The application needs to fetch existing movie details from [https://developers.themoviedb.org/3/getting-started/introduction](https://developers.themoviedb.org/3/getting-started/introduction)

2. A frontend where the user can **play movie**, **bookmark** it and should be able to create **playlist** out of it.
3. Based on the movie played and playlist created the application should be able to recommend with similar movies to the user.

## Modules:
1. AccountManager - Should be able to manage user accounts
2. MuzixUI -
  - User should be able to
    - search movie
    - bookmark movies
    - create playlists
    - should be able to see bookmarked movies and playlists created by him
    - should be able to play the movies
3. MovieManager - Application should be able to store all his
  - bookmarks movies
  - playlists movies
  - searches movies

## Flow of Modules

- **Building Frontend**
  1. Building **Responsive** Views:
    1. Build a View to show all movies
      1. Movies - Populating from external api
      2. Build a view to show created playlist
      3. A view to authenticate users
  2. Using **Services** to populate these data in views
  3. Stitching these views using **Routes and Guards**
  4. E2E test cases and unit test cases
  5. **Writing CI configuration file**
  6. **Dockerizing the frontend**

- **Building the Account Manager**
  1. Creating microservices using Spring Boot and Spring cloud to 
    1. **facilitate registration** and login using **JWT token** and **MySQL**
  2. Writing Swagger Documentation
  3. Unit Testing
  4. Write CI Configuration
  5. Dockerize the application

- **Building the Movies Manager**
  1. Creating microservices using Spring Boot and Spring cloud to 
    1. **facilitate CRUD operation** over movies, playlist and bookmarked resources stored in MySQL and MongoDB
  2. Writing Swagger Documentation
  3. Unit Testing
  4. Write CI Configuration
  5. Dockerize the application
  6. Implement AWS/Azure features to demostrate the knowledge of AWS/Azure cloud

- **Write docker-compose file to build both frontend and backend application**

- **Demonstrate the entire application supported by good presentation using powerpoint/pdf PPT**