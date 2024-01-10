# real-time-chat-nestjs-angular

## Good to know
- Api build with NestJS 8, because v8 has Support for the latest Socket.io Release v4
- Angular used in v12 & also Angular Material
- Start Command `docker-compose up`
- Sometimes the package-lock.json can cause issues, then just delete it and let docker do everything
- In the folder _user_stories you can have a look at all the implemented user stories so far
- Sometimes when you follow the videos you might need to dump the images/containers and rebuild, look below for the tips & tricks
- in the todo.md file are some ideas that could be implemented in the future

## Overview of the Series
This Series is about implementing a Realtime Chat with Websockets (here we used Socket.io v4).
The Main features are:
- Register a new User
- Login with a user and get a valid jwt Token for Auth (API & Websocket)
- Create a Chatroom and add other users by their username
- Join one of your chatrooms and see the latest messages
- Add a message to the chatroom, this will be emitted immediately to all other joined Users for this Room that are currently online

The NestJS API is built with NestJS 8, because v8 has support for the latest socket.io Release v4.

## How to run the Project
Command:  
`docker-compose up`

### Tipps & Tricks
If you follow the videos you something have to delete the images & containers and then start everything again.

Command to remove all images:  
`docker rmi -f $(docker images -a -q)`

Command to remove all containers:  
`docker rm -vf $(docker ps -a -q)`

### Docker commands

Command to start:  
`docker-compose up`

Command to build:
`docker-compose build`


Command to remove all images:  
`docker rmi -f $(docker images -a -q)`

Command to remove all containers:  
`docker rm -vf $(docker ps -a -q)`
