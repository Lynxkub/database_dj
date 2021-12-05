\```sql
1. SELECT titles FROM movies;
2. SELECT * FROM movies WHERE rating = 'G';
3. SELECT title, release_year FROM movies ORDER BY release_year DESC;
4. SELECT * FROM movies ORDER BY runtime DESC LIMIT 5;
5. SELECT rating, COUNT(*) as total FROM movies GROUP BY rating;
6. SELECT release_year, AVG(runtime) AS average_runtime FROM movies GROUP BY release_year ORDER BY release_year DESC;
7. SELECT title, name FROM movies JOIN studios ON movies.studio_id = studios.id;
8. SELECT movies.title, stars.first_name, stars.last_name FROM movies JOIN roles ON movies.id = roles.id JOIN s
tars on roles.star_id = stars.id;
9. SELECT DISTINCT stars.first_name, stars.last_name FROM stars JOIN movies ON rating = 'G';
10. SELECT DISTINCT stars.first_name, stars.last_name FROM stars JOIN roles ON stars.id = roles.id JOIN movies O
N movies.id = roles.movie_id;

\```