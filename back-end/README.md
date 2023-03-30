# TechNative Backend Developer exercise

> The goal is to develop a [Github API](https://docs.github.com/en/rest/repos/repos?apiVersion=2022-11-28) emulator server

This exercise is designed to test your skills in building a Github API emulator server using Express, a database, and authentication. The server should handle all CRUD operations for repositories, and the data should be retrieved from a database. It should support pagination and authentication for secure access.

## Requirements

- Build an Express server that emulates the Github API, but only for repositories.
- Retrieve the repository data from a database that you will first need to create using the data in the [`assets/data.json`](./assets/data.json) file.
- Implement pagination to limit the number of results returned in a single request.
- Add authentication for secure access to the API. Users should be able to log in using a username and password, and only authenticated users should be able to access the API.

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

> These tasks are not required. Please attempt any of them, only if you didn’t spend too much time on the main tasks.

- Write the code in TypeScript.
- Add a graphQL endpoint to the server.
- Implement a caching mechanism to improve the performance of the API.
- Implement a rate limiter to limit the number of requests a user can make in a given time period.
- Deploy the server publicly using a service such as [Render](http://render.com) or AWS.
