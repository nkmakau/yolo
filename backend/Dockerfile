FROM node:latest

LABEL Noah Makau <noshkim78@gmail.com>

COPY . /backend
WORKDIR /backend
RUN npm install

EXPOSE 5000
CMD [ "npm", "start" ]