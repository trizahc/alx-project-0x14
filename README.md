# CineSeek Movie App

## API Overview

The CineSeek app integrates the MoviesDatabase API to fetch and display movie information. This API provides access to a large collection of movie titles, images, genres, and release years. It supports filtering by release year and genre, pagination, and search capabilities, making it ideal for modern movie discovery applications.

## API Version

**v1** (as of the latest documentation)

## Available Endpoints

- `GET /titles`  
  Fetches a list of movie titles. Supports filters such as year, genre, and pagination.

- `GET /titles/{id}`  
  Fetches detailed information about a single movie by its ID.

- `GET /genres`  
  Returns a list of available genres for filtering.

- `GET /years`  
  Returns a list of years that can be used to filter movies by release date.

## Request and Response Format

### Example Request:

```http
GET https://moviesdatabase.p.rapidapi.com/titles?year=2023&genre=Comedy&page=1
Headers:
  x-rapidapi-host: moviesdatabase.p.rapidapi.com
  x-rapidapi-key: YOUR_API_KEY
# alx-project-0x14