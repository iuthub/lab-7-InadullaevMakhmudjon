# Execise 1 Answers

1. SELECT movies.name FROM movies WHERE movies.year = 1995<br/>

2. SELECT COUNT(*) FROM actors JOIN roles ON actors.id = roles.actor_id JOIN movies ON movies.id = roles.movie_id WHERE movies.name = "Lost in Translation"<br/>

3. SELECT actors.first_name, actors.last_name FROM actors JOIN roles ON actors.id = roles.actor_id JOIN movies ON movies.id = roles.movie_id WHERE movies.name="Lost in Translation"<br/>

4. SELECT directors.first_name,directors.last_name FROM directors JOIN movies_directors ON directors.id = movies_directors.director_id JOIN movies ON movies_directors.movie_id = movies.id WHERE movies.name = "Fight Club"<br/>

5. SELECT COUNT(*) FROM movies JOIN movies_directors ON movies_directors.movie_id = movies.id JOIN directors ON movies_directors.director_id = directors.id WHERE directors.first_name="Clint"<br/>

6. SELECT movies.name FROM movies JOIN movies_directors ON movies_directors.movie_id = movies.id JOIN directors ON movies_directors.director_id = directors.id WHERE directors.first_name="Clint"<br/>

7. SELECT directors.first_name,directors.last_name  FROM directors JOIN movies_directors ON movies_directors.director_id = directors.id JOIN movies_genres ON movies_directors.movie_id = movies_genres.movie_id WHERE movies_genres.genre= "horror"<br/>

8. SELECT actors.first_name, actors.last_name FROM actors JOIN roles ON actors.id = roles.actor_id JOIN movies_directors ON roles.movie_id = movies_directors.movie_id JOIN directors ON movies_directors.director_id = directors.id WHERE directors.first_name = "Christopher"<br/>