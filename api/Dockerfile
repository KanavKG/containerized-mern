# Use a lighter version of Node as a parent image
FROM mhart/alpine-node:8.11.4

# Setting the working directory to /api
WORKDIR /api

# copying package.json into the container at /api
COPY package*.json /api/

# installing dependencies
RUN npm install

# Make port 80 available to the world for communication
EXPOSE 80

# Copying the current directory contents into the container at /api
COPY . /api/

ADD https://github.com/ufoscout/docker-compose-wait/releases/download/2.2.1/wait /wait
RUN chmod +x /wait

# Run the app when the container launches
CMD /wait && npm start
