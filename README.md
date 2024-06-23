# API testing - themoviedb.org

The scope of this project is to use all API knowledge gained throught the Software Testing course and apply them in practice, using a live application.

Application under test: themoviedb.org

Tools used: Postman

Link Postman collection run [Git repo screenshot](https://github.com/armandaskalu/API-testing-themoviedb.org/blob/main/TMDB.postman_test_run.json)

## Tests performed

1. GET API Authentication token

HTTP method for request: GET

Request description: using the access token in the Authorization header as a bearer token in order to get a request token in the body section. 

Test types / techniques used: checking response time and status code 

Response status code: 200 OK

Below you can find the message in the response body:

  {  "success": true,
    "expires_at": "2024-06-23 14:20:51 UTC",
    "request_token": "0b548921e1648479d64712215eee111e046c1977"}

JavaScript Tests:

pm.test("Verify if status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Verify if the response time is less than 200ms", function () {
    pm.expect(pm.response.responseTime).to.be.below(200);
});

2. POST New session ID

HTTP method for request: POST

Request description: create a new session id with the athorized request token

Test types / techniques used: checking response time and response body: JSON value check - negative testing (checking if we can get a session ID with an invalid request token)

Response status code: 200 OK

Below you can find the message in the response body:

{ "success": true,
    "session_id": "a8ba9319717c10ae33c86a92a12ebcc1fabc0d67"}

JavaScript Tests:

pm.test("Verify if the response time is less than 400ms", function () {
    pm.expect(pm.response.responseTime).to.be.below(400);
});

pm.test("Verify if it's possible to generate a new session ID with wrong token", function () {
    var jsonData = pm.response.json();
    pm.expect(jsonData.failure).to.eql(true);
});

3. POST Create a list


