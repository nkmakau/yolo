# Base Image
Node:latest-alpine : for both Backend and Client containers.
This image is based on the popular Alpine Linux project, available in the alpine official image. Alpine Linux is much smaller than most distribution base images (~5MB), and thus leads to much slimmer images in general.

Mongo: for the database:
This we did not need to build but pull it directly docker hub.