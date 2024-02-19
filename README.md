# SocialNetExpress

## Description

This repository contains a social network API built using Express.js and MongoDB with Mongoose. The API allows users to share their thoughts, react to friends' thoughts, and manage their friend list.

## Installation

1. Make sure you have MongoDB installed on your machine. Follow the [MongoDB installation guide](https://docs.mongodb.com/manual/installation/) if you haven't already.
2. Clone this repository to your local machine.
3. Navigate to the project directory in your terminal.
4. Run `npm install` to install dependencies.

## Usage

1. Start the server by running `npm start`.
2. Use Insomnia or any other REST client to test the API endpoints.

## API Endpoints

### Users

- `GET /api/users`: Get all users.
- `GET /api/users/:userId`: Get a single user by ID.
- `POST /api/users`: Create a new user.
- `PUT /api/users/:userId`: Update a user by ID.
- `DELETE /api/users/:userId`: Delete a user by ID.

### Friends

- `POST /api/users/:userId/friends/:friendId`: Add a friend to a user's friend list.
- `DELETE /api/users/:userId/friends/:friendId`: Remove a friend from a user's friend list.

### Thoughts

- `GET /api/thoughts`: Get all thoughts.
- `GET /api/thoughts/:thoughtId`: Get a single thought by ID.
- `POST /api/thoughts`: Create a new thought.
- `PUT /api/thoughts/:thoughtId`: Update a thought by ID.
- `DELETE /api/thoughts/:thoughtId`: Delete a thought by ID.

### Reactions

- `POST /api/thoughts/:thoughtId/reactions`: Add a reaction to a thought.
- `DELETE /api/thoughts/:thoughtId/reactions/:reactionId`: Remove a reaction from a thought.

## Walkthrough Video

[Link to Walkthrough Video](https://drive.google.com/file/d/1x1BLkX5fLSJkMXVZUhkPrG4LjjoDX3cQ/view?usp=sharing)

## Bonus

The application automatically deletes a user's associated thoughts when the user is deleted.

## Credits

This project is part of the curriculum of [edX Boot Camps LLC](https://www.edx.org/bootcamps).

## License

This project is licensed under the [MIT License](LICENSE).