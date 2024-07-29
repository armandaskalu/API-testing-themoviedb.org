# API testing - themoviedb.org

The scope of this project is to use all API knowledge gained throught the Software Testing course and apply them in practice, using a live application.

Application under test: themoviedb.org

Tools used: Postman

Link Postman collection run [Git repo screenshot](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/TMDB.postman_test_run.json)

## HTTP methods for requests (GET, POST, DEL) and JavaScripts tests:

1. GET Authentication token
![token](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/1.jpg)
2. POST New session ID
![session](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/2.jpg)
3. POST Create a list
![list](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/3.jpg)
4. GET Display lists
![display](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/4.jpg)
5. POST Add movie to a list
![add](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/5.jpg)
6. DEL Delete a list
![delete](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/6.jpg)
7. GET Search a movie
![search](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/7.jpg)
8. GET Display rated movies
![rated](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/8.jpg)
9. DEL Delete a rating
![del]   

Test types / techniques used: JavaScrispts tests checking response time, status code and response body: JSON value check - positive and negative testing (black box)

Below you can find the execution report that was generated through the Postman collection runner - no defects were found.

![Run Results](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/Results.jpg)


