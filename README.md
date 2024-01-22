# ManyToMany
This is a project for learning Many To Many mapping. 
# Music Library Spring Boot Project

This Spring Boot project demonstrates the implementation of Many-to-Many mapping between `Album` and `Artist` entities in a music library application.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [API Endpoints](#api-endpoints)

## Introduction

The goal of this project is to showcase a Spring Boot application with Many-to-Many mapping, allowing albums to be associated with multiple artists and vice versa in a music library system.

## Features

- **Album Management:**
  - Create, read, update, and delete album details.
  - Associate albums with multiple artists using Many-to-Many mapping.

- **Artist Management:**
  - Create, read, update, and delete artist details.
  - Associate artists with multiple albums using Many-to-Many mapping.

## Technologies Used

- Spring Boot
- Spring Data JPA
- RESTful API
- H2 Database (for demonstration purposes; can be replaced with a production database)
- Maven

## Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Vishwajeet-29-pro/ManyToMany.git

2. **Build and Run the Application:**
   ```bash
   cd ManyToMany
    ./mvnw spring-boot:run

3. **Access the API:**
The application will be accessible at http://localhost:8080.

Album Controller
Create Album:

POST /api/1.0/music/album/
Get All Albums:

GET /api/1.0/music/album/
Get Album by ID:

GET /api/1.0/music/album/{id}
Update Album by ID:

PUT /api/1.0/music/album/updateAlbumDetailsById/{id}
Delete Album by ID:

DELETE /api/1.0/music/album/deleteAlbumDetailsById/{id}
Add Album to Artist:

POST /api/1.0/music/album/{albumId}/addArtist/{artistId}
Remove Album from Artist:

DELETE /api/1.0/music/album/{albumId}/removeArtist/{artistId}
Get All Albums by Artist ID:

GET /api/1.0/music/album/getAllAlbumByArtistId/{id}
Artist Controller
Create Artist:

POST /api/1.0/music/artist/
Get All Artists:

GET /api/1.0/music/artist/
Get Artist by ID:

GET /api/1.0/music/artist/getById/{id}
Update Artist by ID:

PUT /api/1.0/music/artist/updateArtistById/{id}
Delete Artist by ID:

DELETE /api/1.0/music/artist/deleteArtistById/{id}
Add Artist to Album:

POST /api/1.0/music/artist/{artistId}/addAlbum/{albumId}
Remove Album from Artist:

DELETE /api/1.0/music/artist/{artistId}/removeAlbum/{albumId}
Get All Artists by Album ID:

GET /api/1.0/music/artist/getAllAlbumsByArtistId/{id}

