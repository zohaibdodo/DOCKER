#Simple Docker File:

FROM ngnix
COPY . /usr/share/ngnix/html

#Complex Docker File:

FROM alpine
LABEL maintainer="aamirpinger@yahoo.com"
RUN apk add --update nodejs nodejs-npm
COPY . /src
WORKDIR /src
RUN npm install
ENV CREATEDBY="Aamir Pinger"
EXPOSE 8080
ENTRYPOINT ["node","./app.js"]


Create a name.js file:

console.log("Hello Docker!")

Now create a Dockerfile:

FROM node:alpine
COPY . /app
WORKDIR /app
CMD node app.js

Now package our application:

#docker build -t hello-docker .

Now check:

#docker images ls