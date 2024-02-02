# Code Seed Frontend Developer Exercise

> The objective of this exercise is to create a GitHub repository search application.

## Requirements

1. Develop a search interface for users to input a search query.
2. Display a list of repositories matching the search query.
3. Include pagination to navigate through the search results.
4. Display the organization's avatar, repository name, description, and other relevant information for each search result.
5. Implement a "favourites" functionality that allows users to mark repositories as favourites.

## Technical Specifications

- Please develop the application using a modern JavaScript framework (React, Angular, or Vue).
- Aim to match the provided target screenshots in terms of styling and features, but pixel-perfect precision is not required. Create a responsive design that adapts to different screen sizes and orientations.
- You are free to use any libraries (e.g., Jest, styled-components, Lodash), with the exception of component libraries like Material UI. If in doubt, feel free to ask.
- Utilize the following GitHub API endpoint: [https://api.github.com/search/repositories](https://api.github.com/search/repositories)
  - You can find the endpoint documentation here: [https://developer.github.com/v3/search/#search-repositories](https://developer.github.com/v3/search/#search-repositories)
  - There is no need to use the Octokit library suggested in the documentation; feel free to use any library you are comfortable with.
  - Be mindful of the GitHub API's quota limitations; you don't need to handle them, but please be aware of their existence.
- You may use any familiar project setup tool (e.g., create-react-app, angular-cli, vue-cli), but we recommend using [Vite](https://vitejs.dev/), a zero-config bundler that is simple to use.

## Bonus Tasks

1. Implement sorting functionality for search results (e.g., by stars, forks, or recently updated).
2. Add filters for the search results (e.g., language, license, creation date).
3. Write unit and integration tests for your application.
4. Use TypeScript for type checking and improved code quality.
5. Add persistence to the "favourites" functionality, allowing users to maintain their list of favourite repositories across sessions.
