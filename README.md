# Book-Search-Engine

## Description

The **Book-Search-Engine** project involves refactoring an existing Google Books API search engine to use GraphQL with Apollo Server. The application is built using the MERN stack, with a React front end, MongoDB database, and Node.js/Express.js server. The app allows users to search for books, save their favorite books to their account, and manage their saved book list. This refactor enhances the performance and usability of the application by transitioning from RESTful API practices to GraphQL.

## User Story


AS AN avid reader
I WANT to search for new books to read
SO THAT I can keep a list of books to purchase

## Project Structure

- **server.js**: Configures Apollo Server and integrates it with the Express.js server.
- **auth.js**: Contains updated authentication middleware to work with GraphQL.
- **Schemas**: Directory containing the GraphQL schema definitions and resolvers.
  - **index.js**: Exports typeDefs and resolvers.
  - **typeDefs.js**: Defines the GraphQL types, queries, and mutations.
  - **resolvers.js**: Implements the functionality for the defined queries and mutations.
- **client/src**: Front-end React components and utilities.
  - **App.jsx**: Sets up Apollo Provider for the app.
  - **SearchBooks.jsx**: Handles book search functionality with GraphQL mutations.
  - **SavedBooks.jsx**: Manages the display and removal of saved books using GraphQL queries and mutations.
  - **SignupForm.jsx**: Manages user signup using GraphQL mutations.
  - **LoginForm.jsx**: Manages user login using GraphQL mutations.
  - **queries.js**: Contains GraphQL query for fetching user data.
  - **mutations.js**: Contains GraphQL mutations for login, signup, save book, and remove book actions.

## Improvements Made

- Refactored the RESTful API to use GraphQL with Apollo Server.
- Updated the authentication middleware to support GraphQL.
- Integrated Apollo Client in the React front end to handle queries and mutations.
- Deployed the application to Render with a MongoDB database hosted on MongoDB Atlas.

## Deployment

The project is deployed on Render and can be accessed at the following URL:

[Link to deployed project](https://book-search-engine-22v1.onrender.com/)

## Contributions

Contributions are welcome. If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/new-feature`).
3. Make the necessary changes and commit them (`git commit -m 'Add new feature'`).
4. Push the changes to your repository (`git push origin feature/new-feature`).
5. Create a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
