FROM ubuntu:16.04

WORKDIR /
COPY frontend-example-docker /frontend/

RUN apt-get update && apt-get install curl -y
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install -g serve
EXPOSE 5000

WORKDIR /frontend/
CMD API_URL=http://localhost:8000 npm start