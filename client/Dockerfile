# build environment
FROM node:13.12.0-alpine AS client

LABEL version="1.0"
LABEL description="This is client base docker image"
LABEL maintainer="Noah Makau <noshkim78@gmail.com>"

WORKDIR /usr/src/client

COPY package*.jason ./

RUN npm install
COPY . .

RUN npm run build
RUN npm install -g serve

EXPOSE 3000
CMD ["serve","-s", "build", "-l", "3000"]