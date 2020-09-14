FROM node:13.12.0-alpine as backend

LABEL version="2.0"
LABEL description="This is backend base docker image"
LABEL maintainer="Noah Makau <noshkim78@gmail.com>"

ENV PATH /backend/node_modules/.bin:$PATH 

COPY . /backend
WORKDIR /backend
RUN npm install

EXPOSE 5000
CMD [ "npm", "start" ]