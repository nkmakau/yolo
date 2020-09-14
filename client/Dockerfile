# build environment
FROM node:13.12.0-alpine AS client

LABEL version="1.0"
LABEL description="This is client base docker image"
LABEL maintainer="Noah Makau <noshkim78@gmail.com>"


ENV PATH /client/node_modules/.bin:$PATH

COPY . /client
WORKDIR /client
RUN npm install
RUN npm run build
RUN npm install -g serve

EXPOSE 3000
CMD ["serve","-s", "build", "-l", "3000"]