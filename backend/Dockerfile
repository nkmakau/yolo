FROM node:latest

LABEL version="1.0"
LABEL description="This is our base docker image"
LABEL maintainer="Noah Makau <noshkim78@gmail.com>"

COPY . /backend
WORKDIR /backend
RUN npm install

EXPOSE 5000
CMD [ "npm", "start" ]