# Base Image
Node:latest-alpine : for both Backend and Client containers.
This image is based on the popular Alpine Linux project, available in the alpine official image. Alpine Linux is much smaller than most distribution base images (~5MB), and thus leads to much slimmer images in general.

Mongo: for the database:
This we did not need to build but pull it directly docker hub.

# Docker Directives
Used the following 
FROM sets base images for backend, client and mongo
COPY copies files to containers
RUN initiates commands to install and build
WORKDIR holds files for the current directory
EXPOSE opens up ports for apps
Network builds the intercontainer network
CMD commands to fire up our app
LABEL gives decription, names, version to our images

VOLUME

# Docker-compose Networking
Build a bridge network titled nosh-yolo linking the 3 containers

# Docker-compose Volume
Used volume have called mongodata to hold DB data.
seats in var/lib/shared/mongodata

# Git workflow
Changed remote repo to nkmakau
git commits done for every dockerfile and docker-compose added and any other change made
pushed changes to new repo.

# Bugs
No bugs noted in case of any kindly contact author.


# Docker image tag
Images are tagged with the name of the application:
mongo - for mongodb
yolo-client is tagged as noshmak/client
yolo-backend is tagged as noshmak/backend

Containers are also tagged the same:
nosh_mongo for the database
nosh_client for frontend
nosh_backend for the backend

# Docker Hub Images
[Yolo Client](https://hub.docker.com/r/noshmak/client)

[Yolo Backend](https://hub.docker.com/r/noshmak/backend)

# Prerequistes
Docker
Docker Compose

# Instructions
Run the followind commands on terminal to build the app on docker
    git clone https://github.com/noshmak/yolo.git
    cd yolo
    docker-compose up --build
    Access App on http://localhost:3000