# Introvoke Backend Interview

Welcome to the Introvoke backend developer interview project! 👋

## Objective

Your assignment is to implement a chat API server that will allow for creating new messages, getting all messages, getting a single message, updating a single message, and deleting a single message.

Feel free to use any tools to help aid you in completing this assignment.

## Tasks

- Implement using the following:
  - Recommended Language: Typescript/JavaScript (NodeJS)
- The API should expose endpoints which satisfy the following:
  - Creating a new chat message
  - Updating an existing chat message
  - Getting an existing chat message
  - Getting all chat messages
  - Deleting a chat message
- The chat messages should have the following properties:
  - A unique ID
  - The text of the chat message
  - The username of the user who sent the message
  - The time the message was created and/or updated

You may also create any additional routes that you believe would be beneficial.

Your API should follow REST methodology for managing the state of the chat messages. Below is what is expected when calling your API endpoints:

- All requests that take or return a body payload must be of content type `application/json`
- It is expected that all routes return expected status codes and payloads respective to their operations
  - Example: A user makes a `POST` request to your API with a missing property, it is expected that your API return an error status code and optional error message in the body

### Bonus

- Add validation to user inputs
- Validate your code and components through testing using any test frameworks of your choice
- Think of ways we can authenticate the API and prevent bad actors
- Think of ways to monitor the API for errors, invalid requests, timeouts

### Testing

To test your API routes we recommend using an API tool such as [Postman](https://www.postman.com/) to easily and quickly test your endpoints as you create them.

We have also provided a [Postman collection](/Backend%20Interview%20Project.postman_collection.json) which you can use to test your routes. You may update this collection to suit your needs.

## Getting Started

This project is currently setup with [Docker](https://www.docker.com/) and (Docker Compose)[https://docs.docker.com/compose/]. The `/server` directory contains a ready-to-go NodeJS Typescript project that will auto-reload when changes are made. If you wish to use a different language or your own environment, feel free to start from scratch.

To start, let's build and run the docker container. From the root of this directory, run the following command:

```bash
docker-compose build
```

This will build the docker container image and automatically run the NPM install script for the server within the server Docker container.

Next, we can start the containers using the following:

```bash
docker-compose up
```

After a few seconds you should see `Hello World!` printed in the console output. You are now ready to get started!

The the [Server README](/server/README.md) file contains additional information for creating your server.
