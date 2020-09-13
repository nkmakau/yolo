FROM node:latest

LABEL Noah Makau <noshkim78@gmail.com>

COPY . /backend
WORKDIR /yolo
RUN npm install

EXPOSE 5000
CMD [ "npm", "start" ]