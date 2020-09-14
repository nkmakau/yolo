FROM node:13.12.0-alpine as backend

LABEL version="2.0"
LABEL description="This is backend base docker image"
LABEL maintainer="Noah Makau <noshkim78@gmail.com>"

WORKDIR /backend
COPY . /backend

RUN npm install
EXPOSE 5000
CMD [ "npm", "start" ]