# Base Image
Node:latest-alpine : for both Backend and Client containers.
This image is based on the popular Alpine Linux project, available in the alpine official image. Alpine Linux is much smaller than most distribution base images (~5MB), and thus leads to much slimmer images in general.

Mongo: for the database:
This we did not need to build but pull it directly docker hub.

# Docker Directives
Used the following 
FROM
COPY
RUN
WORKDIR
EXPOSE
ENV
CMD
LABEL

VOLUME

# Docker-compose Networking
Build a network titled yolo-network linking the 3 containers

# Docker-compose Volume
Used yolo-volume
seats in var/lib/shared/yolo

# Git workflow
Changed remote repo to nkmakau
git commits done for every dockerfile and docker-compose added and any other change made
pushed changes to new repo.

# Bugs
No bugs noted in case of any kindly contact author.


# Docker image tag
Images are tagged with the name of the application:
mongo - for mongodb
yolo-client for front end image
yolo-backend for bankend image.

Containers are also tagged the same:
yolo_mongo_1 for the database
yolo_client_1 for frontend
yolo_backend_1 for the backend
