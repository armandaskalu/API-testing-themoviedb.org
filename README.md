# API testing - themoviedb.org

The scope of this project is to use all API knowledge gained throught the Software Testing course and apply them in practice, using a live application.

Application under test: themoviedb.org

Tools used: Postman

Link Postman collection run [Git repo screenshot](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/TMDB.postman_test_run.json)

## HTTP methods for requests: GET, POST, DEL

1. GET Authentication token
![token](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/1.jpg)
2. POST New session ID
![session]
3. POST https://api.themoviedb.org/3/list?session_id=5a3c2d02675d3015c0f90e0cac87db3565a43cdb (Create a list)

4. GET https://api.themoviedb.org/3/account/21294757/lists?page=1&session_id=5a3c2d02675d3015c0f90e0cac87db3565a43cdb (Display lists)

5. POST https://api.themoviedb.org/3/list/8302327/add_item?session_id=619a1e58931c6edd39267f40ca2bc781321fb7e0 (Add movie to a list)

6. DEL https://api.themoviedb.org/3/list/8302332?session=619a1e58931c6edd39267f40ca2bc781321fb7e0 (Delete a list)

7. GET https://api.themoviedb.org/3/search/movie?query=fifth element&include_adult=false&language=en-US&primary_release_year=&page=1&region=USA&year= (Search a movie)

8. POST https://api.themoviedb.org/3/account/21294757/watchlist?session_id=619a1e58931c6edd39267f40ca2bc781321fb7e0 (Add movie to watchlist)

9. GET https://api.themoviedb.org/3/account/21294757/watchlist/movies (Display watchlist movies)

10. POST https://api.themoviedb.org/3/account/21294757/favorite?session_id=5a3c2d02675d3015c0f90e0cac87db3565a43cdb (Add movie to favorites)

11. GET https://api.themoviedb.org/3/account/21294757/favorite/movies (Dispaly favorite movies)

12. POST https://api.themoviedb.org/3/movie/614933/rating?session_id=619a1e58931c6edd39267f40ca2bc781321fb7e0 (Add rating)

13. DEL https://api.themoviedb.org/3/movie/18/rating (Delete a rating)

14. GET https://api.themoviedb.org/3/account/21294757/rated/movies (Display rated movies)

Test types / techniques used: JavaScrispts tests checking response time, status code and response body: JSON value check - positive and negative testing (black box)

Below you can find the execution report that was generated through the Postman collection runner - no defects were found.

![Run Results](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/Results.jpg)


