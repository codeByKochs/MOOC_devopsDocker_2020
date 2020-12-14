FROM ubuntu:16.04

WORKDIR /
COPY frontend-example-docker /frontend/

RUN apt-get update && apt-get install curl -y && \
    curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    apt install -y nodejs && \
    npm install -g serve && \
    apt-get purge -y --auto-remove curl && \ 
    rm -rf /var/lib/apt/lists/* 

EXPOSE 5000

WORKDIR /frontend/
CMD npm start