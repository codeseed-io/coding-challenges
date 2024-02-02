# Code Seed Backend Developer exercise

> The goal is to develop a simpler [Github API](https://docs.github.com/en/rest/repos/repos?apiVersion=2022-11-28) emulator server

This exercise is designed to test your skills in building a simpler Github API emulator server using Express, a database, and authentication. The server should handle basic CRUD operations for repositories, and the data should be retrieved from a database.

## Requirements

- Build an Express server that emulates the Github API, but only for repositories.
- Retrieve the repository data from a database that you will first need to create using the data in the [`assets/data.json`](./assets/data.json) file.
- Implement pagination to limit the number of results returned in a single request and support filtering based on the repository owner.
- Add authentication for secure access to the API. Users should be able to log in using a username and password, and only authenticated users should be able to access the API.

## Routes

1. `GET /api/repositories`: Retrieve a list of repositories with pagination support and owner-based filtering. Returns a JSON array of repository objects.
2. `POST /api/repositories`: Create a new repository. Expects a JSON object containing the repository details in the request body. Returns the created repository object.
3. `GET /api/repositories/:full_name`: Retrieve a single repository by its full name (e.g., owner/repository_name). Returns the repository object.
4. `PUT /api/repositories/:full_name`: Update a repository by its full name. Expects a JSON object containing the updated repository details in the request body. Returns the updated repository object.
5. `DELETE /api/repositories/:full_name`: Delete a repository by its full name. Returns a success message upon successful deletion.
6. `POST /api/auth/login`: Authenticate a user. Expects a JSON object containing the username and password in the request body. Returns an access token upon successful authentication.

> **Note** \
> You don't have to follow the Github API specification to the letter. The routes provided above are just examples of possible routes for this simplified version. Feel free to come up with your own routes and design choices as long as you meet the main requirements of the exercise.

## Technical Specifications

- Use Express.js as the server framework.
- Use MongoDB, or any other SQL or NoSQL database, to store the repository data.
- Use a popular authentication method, such as JWT or OAuth2.
- Use pagination to limit the number of results returned in a single request.
- Write clean and maintainable code.
- Use ESLint to ensure the code follows a consistent style and prettier to format the code.
- Implement error handling to handle any errors that may arise.
- Write unit tests to ensure the server is working correctly.

### Bonus Tasks

> **Warning** \
> These tasks are not required. Please attempt any of them, only if you didn’t spend too much time on the main tasks.

- Write the code in TypeScript.
- Add a graphQL endpoint to the server.
- Implement a caching mechanism to improve the performance of the API.
- Implement a rate limiter to limit the number of requests a user can make in a given time period.
- Deploy the server publicly using a service such as [Render](http://render.com) or AWS.
