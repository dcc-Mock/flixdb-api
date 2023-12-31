# FlixDB API

This repository contains static JSON data that's served up through My JSON Server as a read-only API. 

db.json holds an object with a movies property, containing an array of movie objects. This "movies" property becomes a GET endpoint via My JSON Server. The Flix API endpoints return supplemental data for the Movies API, used in the React tutorial series.

## /movies

The movies endpoint contains data for the following movies:
- The Dark Knight
- Inception
- Interstellar
- The Shawshank Redemption
- The Godfather
- The Matrix
- Avatar
- Titanic
- The Avengers
- The Terminator
- Star Wars: A New Hope
- Jaws
- Fight Club
- Schindler's List

### Collection

**GET**: `http://my-json-server.typicode.com/dCC-Mock/flixdb-api/movies`

Response:
```
[
  {
      "id": "The Dark Knight",
      "poster_url": "https://image.tmdb.org/t/p/w500/1hRoyzDtpgMU7Dz4JF22RANzQO7.jpg",
      "release_date": "2008-07-18"
  },
  {
      "id": "Inception",
      "poster_url": "https://image.tmdb.org/t/p/w500/9gk7adHYeDvHkCSEqAvQNLV5Uge.jpg",
      "release_date": "2010-07-16"
  }
  ...
]
```

### Detail

**GET**: `http://my-json-server.typicode.com/dCC-Mock/flixdb-api/movies/The Dark Knight`

Response:
```
{
  "id": "The Dark Knight",
  "poster_url": "https://image.tmdb.org/t/p/w500/1hRoyzDtpgMU7Dz4JF22RANzQO7.jpg",
  "release_date": "2008-07-18"
}
```


