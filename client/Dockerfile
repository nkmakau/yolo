# build environment
FROM node:latest

LABEL Noah Makau <noshkim78@gmail.com>

COPY . /client
WORKDIR /yolo
RUN npm install
RUN npm run build
RUN npm install -g serve

EXPOSE 3000
CMD ["serve","-s", "build", "-l", "3000"]