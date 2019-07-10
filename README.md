## About the app
Actually, there are two separated apps. The Client which serves the FrontEnd (using React), and the API (in Node/Express).

## How to run the API
1. In your terminal, navigate to the `api` directory.
2. Run `npm install` to install all dependencies.
3. Run `npm start` to start the app.

## How to run the Client
1. In another terminal, navigate to the `client` directory.
2. Run `npm install` to install all dependencies.
3. Run `npm start` to start the app

## Check if they are connected
1. With the two apps running, open your browser in http://localhost:3000/.
2. If you see a webpage saying `Welcome to React`, it means the FrontEnd is working.
3. If the same webpage has the phrase `API is working properly`, it means the API is working.
=======
# docker-mern-boilerplate

Docker-compose commands: 

FROM

The base image for building a new image. This command must be on top of the dockerfile.

MAINTAINER

Optional, it contains the name of the maintainer of the image.

RUN

Used to execute a command during the build process of the docker image.

ADD

Copy a file from the host machine to the new docker image. There is an option to use an URL for the file, docker will then download that file to the destination directory.

ENV

Define an environment variable.

CMD

Used for executing commands when we build a new container from the docker image.

ENTRYPOINT

Define the default command that will be executed when the container is running.

WORKDIR

This is directive for CMD command to be executed.

USER

Set the user or UID for the container created with the image.

VOLUME

Enable access/linked directory between the container and the host machine.
