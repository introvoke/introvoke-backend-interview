# Server API

This is a pre-configured TypeScript project that will auto-reload when changes are made to your code.

To run this project locally on your machine (not in a container), simply run the following commands from this directory:

```bash
npm install && npm start
```

You will see the following printed out in the console:

```bash
$ Hello World!
```

Feel free to use any frameworks or tools to aid you in completing this project. If you wish to use a different language, you may remove these files and start from scratch. If you wish to use the Docker container setup, update the Dockerfile in this directory with any additional things you may need.

## Running in a container

If running the server within a Docker container, you may change your code and install dependencies as you would normally. The compose file links the volume within this directory to allow for changes to instantly update the code within the container.

You may also connect to the MongoDB database container from the server container by using the following URI: `mongodb://mongo:27017`. Checkout the [Docker Compose YAML file](../docker-compose.yml) for information on current configurations.
